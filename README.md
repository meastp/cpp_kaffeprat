# cpp_kaffeprat

# C++ Core Guidelines

https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines

# presentasjoner

- http://meastp.github.io/cpp_kaffeprat/1.html
- http://meastp.github.io/cpp_kaffeprat/2.html
- http://meastp.github.io/cpp_kaffeprat/3.html
- http://meastp.github.io/cpp_kaffeprat/4.html
- http://meastp.github.io/cpp_kaffeprat/5.html
- http://meastp.github.io/cpp_kaffeprat/6.html
- http://meastp.github.io/cpp_kaffeprat/7.html

# status

```cpp
using namespace std;
```
## C++11
 - [x] (1) nullptr
 - [x] (1) auto
 - [x] (1) to_string
 - [x] (1) tie, tuple
 - [x] (1) array
 - [x] (1) range-based for
 - [x] (1) unique_ptr, make_unique
 - [x] (1) shared_ptr, make_shared
 - [x] (2) non-static data member initializers
 - [x] (2) move semantics: move, forward, rvalue references og move constructors/-assignment
 - [x] (2) default and deleted functions
 - [x] (3) enum class ("strongly typed enums")
 - [x] (3) using (i stedet for typedef) (alias og alias templates)
 - [x] (3) lambda-funksjoner
 - [x] (4) override og final
 - [] (5) std::mutex, std::recursive_mutex osv.
 - [] (5) std::lock, std::lock_guard
 - [] (5) std::atomic
 - [] (5) std::thread
 - [] (5) std::future
 - [] (6) inline-namespace
 - [] (6) user-defined literals
 - [] (6) initializer lists
 - [] (6) delegating constructors
 - [] (6) std::chrono
 - [ ] (7) attributes
 - [ ] (7) decltype
 - [ ] (7) type traits (eks. std::is_integral<int>::value)
 - [ ] (7) variadic templates
 - [ ] constexpr

## C++14
 - [ ] constexpr med færre begrensninger
 - [ ] user-defined literals for standard library types
 - [ ] binary literals
 - [ ] lambda capture initializers
 - [ ] generic lambda expressions
 - [ ] variable templates
 - [ ] return type deduction
 - [ ] decltype(auto)
 - [ ] std::integer_sequence

## C++17
 - [ ] std::filesystem
 - [ ] std::variant
 - [ ] std::optional
 - [ ] std::any
 - [ ] std::string_view
 - [ ] std::invoke
 - [ ] std::apply
 - [ ] splicing for maps and sets
 - [ ] template argument deduction for class templates
 - [ ] declaring non-type template parameters with auto
 - [ ] folding expressions
 - [ ] constexpr lambda
 - [ ] lambda capture this by value
 - [ ] inline variables
 - [ ] nested namespaces
 - [ ] structured bindings
 - [ ] selection statements (if og switch) with initializer
 - [ ] constexpr if
 - [ ] utf-8 character literals

## C++20 TBD
 - [ ] Concepts
 - [ ] Ranges
 - [ ] Modules
 - [ ] Contracts
 - [ ] operator<=>
 - [ ] range-based for with initializer
 - [ ] synchronized buffered ostream
 - [ ] flere constexpr-funksjoner i std
 - [ ] floating-point atomics
 - [ ] starts_with() and ends_with() for strenger
 - [ ] template-parametre for lambdaer
 - [ ] designated initializers
 - [ ] detecting endianness programmatically
 - [ ] make_shared for arrays

## C++ Technical Specifications
 - [ ] Parallelism (v1 og v2)
 - [ ] Transactional Memory (v1 og v2)
 - [ ] Library Fundamentals (v1 og v2)
 - [ ] Concurrency (v1 og v2)
 - [ ] Coroutines
 - [ ] Networking
 - [ ] Reflection
 - [ ] Numerics
 - [ ] Graphics
