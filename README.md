# cpp_kaffeprat

# C++ Core Guidelines

https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines

# presentasjoner

- http://meastp.github.io/cpp_kaffeprat/presentation.html?file=1.md
- http://meastp.github.io/cpp_kaffeprat/presentation.html?file=2.md
- http://meastp.github.io/cpp_kaffeprat/presentation.html?file=3.md
- http://meastp.github.io/cpp_kaffeprat/presentation.html?file=4.md
- http://meastp.github.io/cpp_kaffeprat/presentation.html?file=5.md
- http://meastp.github.io/cpp_kaffeprat/presentation.html?file=6.md
- http://meastp.github.io/cpp_kaffeprat/presentation.html?file=7.md
- http://meastp.github.io/cpp_kaffeprat/presentation.html?file=8.md

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
 - [x] (5) std::mutex, std::recursive_mutex osv.
 - [x] (5) std::lock, std::lock_guard
 - [x] (5) std::atomic
 - [x] (5) std::thread
 - [x] (5) std::future
 - [x] (6) inline-namespace
 - [x] (6) user-defined literals
 - [x] (6) initializer lists
 - [x] (6) delegating constructors
 - [x] (6) std::chrono
 - [x] (7) attributes
 - [x] (7) decltype
 - [x] (7) type traits (eks. std::is_integral<int>::value)
 - [x] (7) variadic templates
 - [x] (8) constexpr

## C++14
 - [x] (8) constexpr med færre begrensninger
 - [x] (8) user-defined literals for standard library types
 - [x] (8) binary literals
 - [x] (8) lambda capture initializers
 - [x] (8) generic lambda expressions
 - [x] (8) return type deduction
 - [x] (8) decltype(auto)
 - [x] (8) std::integer_sequence
 - [x] (8) variable templates

## C++17
 - [ ] (9) nested namespaces
 https://en.cppreference.com/w/cpp/language/namespace
 
 namespace A::B::C { }
 namespace A { namespace B { namespace C { }}}
 
 - [ ] (9) utf-8 character literals
 https://en.cppreference.com/w/cpp/language/character_literal
 
 u8'a' (krever MSVC /utf8 kompilator-parameter)
 
 - [ ] (9) splicing for maps and sets (insert_or_assign, try_emplace, merge, extract)
 https://www.modernescpp.com/index.php/c-17-the-improved-interface-of-the-associative-containers
 
 - [ ] (9) inline variables

// erstatter også extern const-variable

struct MyClass
{
    inline static const int sValue = 777;
};
 
 - [ ] (9) std::optional
 https://en.cppreference.com/w/cpp/utility/optional
 
 auto o1 = std::optional<int>{};
 auto o2 = std::optional<int>{42};
 
 assert(!o1);
 assert(o2);
 
 *o1 // krasj
 *o2 // 42
 
 - [ ] (9) std::any
 https://en.cppreference.com/w/cpp/utility/any
 
 Er en eiende void* som er type-sikker.
 
 - [ ] (9) std::filesystem
 https://en.cppreference.com/w/cpp/filesystem
 
 
 - [ ] std::string_view
 https://en.cppreference.com/w/cpp/string/basic_string_view
 
 https://devblogs.microsoft.com/cppblog/stdstring_view-the-duct-tape-of-string-types/
 
 En ikke-eiende referanse til en string
 
 - [ ] std::variant, std::visit
 - [ ] structured bindings
 - [ ] selection statements (if og switch) with initializer
 - [ ] std::apply
 - [ ] std::invoke
 - [ ] folding expressions
 - [ ] template argument deduction for class templates
 - [ ] declaring non-type template parameters with auto
 - [ ] constexpr if
 - [ ] constexpr lambda
 - [ ] lambda capture this by value

## Oppsummering Unicode

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
