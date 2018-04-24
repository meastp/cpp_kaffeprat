# C++11

---

## nullptr

Dette er en null-peker, og *skal* brukes i stedet for NULL.

http://en.cppreference.com/w/cpp/language/nullptr

---
## auto

Dette er kanskje den mest synlige nyheten i C++11, og brukes der typen *ikke* skal konverteres.

Ved å bruke *auto* sikrer man seg også ved refaktorering, fordi det blir færre steder å gjenta typen.

**C++11**
```cpp

std:string& getName();

auto name1 = getName(); // name1 er std::string

auto& name2 = getName(); // name2 er std::string&

const auto& name3 = getName(); // name3 er const std::string&

```

http://en.cppreference.com/w/cpp/language/auto

---
## auto (forts.)
Overgang til *long long* (64bit) vil være sikrere ved bruk av auto, fordi det mye mindre sjanse for å glemme et sted funksjonen er brukt, slik at verdien blir trunkert.

**C++**
```cpp
int getPersistentID() const;

/// ...

int pid = getPersistentID(); 
// Hvis funksjonen endres til å returnere long long
long long getPersistentID() const;
// vil verdien bli trunkert til 32 bit.
```

**C++11**
```cpp
int getPersistentID() const;

/// ...

auto pid = getPersistentID();
// Hvis funksjonen endres til å returnere long long
long long getPersistentID() const;
// vil verdien beholdes uten konvertering/trunkering her
```

http://en.cppreference.com/w/cpp/language/auto

---

## std::to_string

Konverterer et tall til *std::string*

```cpp
auto str = std::to_string(42);
auto str2 = std::to_string(42.0);
auto str3 = std::to_string(42LL);
```

http://en.cppreference.com/w/cpp/string/basic_string/to_string

---
## std::tuple og std::tie

*tuple* er en hetrogen liste med verdier (forskjellige typer).

Den er særlig mye brukt til template/compile-time programmering, fordi den kan manipuleres og inspiseres.

```cpp
std::tuple<int, std::string, int> t1;

auto t2 = std::make_tuple(1, "str", 3);

int a, c;
std::string b;

std::tie(a, b, c) = t2;

int x, z;

std::tie(x, std::ignore, z) = t2;
```

http://en.cppreference.com/w/cpp/utility/tuple
http://en.cppreference.com/w/cpp/utility/tuple/tie

---
## range-based for

Dette er en for-each-løkke, og kan brukes på alle objekter med **begin()**- og **end()**-funksjoner.

(Enten som medlemsfunksjoner, eller frittstående **std::begin()** og **std::end()**)

**C++**
```cpp
std::vector<int> vec;

for(std::vector<int>::iterator it=vec.begin();it<vec.end();++it)
{
  std::cout << *it;
}
```

**C++11**
```cpp
std::vector<int> vec;

for(auto val: vec)
{
  std::cout << val;
}
```

http://en.cppreference.com/w/cpp/language/range-for

---

## std::array

Dette er et array på *stack* med *statisk* størrelse (med iteratorer, størrelse osv.), 
og *skal* brukes i stedet for C-array.

**C++**
```cpp
char buf[1024];
const int BUFFER_SIZE = 1024;

for(auto i=0;i<BUFFER_SIZE;++i)
{
  buf[i} = 'a';
}
```

**C++11**
```cpp
std::array<char,1024> buffer;


for(auto& val: buffer)
{
  val = 'a';
}
```

http://en.cppreference.com/w/cpp/container/array

---
## pekere i C++98 (raw pointers)

Et stort problem med pekere er at det er umulig å vite hvilken kopi av pekeren som "eier" den. 
Da blir det umulig å vite hvor pekeren skal slettes.

C++98
```cpp
class NumInterface
{
int* getNumber();
void setNumber(int* num);
}

NumInterface& interface = // ...

auto i = interface.getNumber();

// skal i slettes, eller er det bare et "view"/en observatør?

int* p = new int(5);

interface.setNumber(p);

// skal p slettes, eller har interface tatt over "eierskapet"?

```

http://en.cppreference.com/w/cpp/memory/unique_ptr

---
## std::unique_ptr og std::make_unique

I C++11 har vi fått *unique_ptr* som brukes der det til enhver tid er kun én eier av objektet. Denne kan dermed ikke kopieres, men må flyttes (jf. *move semantics* og *rvalue references*, som også er nytt).

**C++11**
```cpp
auto name = std::make_unique<QdiStringAttribute>("name", nullptr, "value");

// unique_ptr "eier" nå pekeren, slik at den slettes når name går ut av scope

auto name_observer = name.get() // get() returnerer QdiStringAttribute*

auto name_observer2 = *name // * fungerer likt som en "raw" peker

auto name_new_owner = name.release() // release()-funksjonen flytter eierskapet til en "raw" peker, for kompabilitet med C++98

```

http://en.cppreference.com/w/cpp/memory/unique_ptr
http://en.cppreference.com/w/cpp/memory/unique_ptr/make_unique

---
## std::shared_ptr og std::make_shared

Vi har også fått *shared_ptr* som brukes der det er mer enn én eier av objektet på én gang. Denne kan dermed kopieres, men er selvfølgelig tregere enn *unique_ptr* - bruk *unique_ptr* hvis ikke *shared_ptr* er nødvendig.

**C++11**
```cpp
auto name = std::make_shared<QdiStringAttribute>("name", nullptr, "value");
auto name2 = name;

// name og name2 "eier" nå pekeren, slik at den slettes når alle kopier går ut av scope

auto name_observer = name.get() // get() returnerer QdiStringAttribute*

auto name_observer2 = *name // * fungerer likt som en "raw" peker

func(const shared_ptr<QdiStringAttribute>&); // Sender inn shared_ptr by-reference. Pass på at en annen shared_ptr holder pekeren i live.

func(shared_ptr<QdiStringAttribute>); // kopierer shared_ptr og holder dermed pekeren i live på egen hånd

```

http://en.cppreference.com/w/cpp/memory/shared_ptr
http://en.cppreference.com/w/cpp/memory/shared_ptr/make_shared
