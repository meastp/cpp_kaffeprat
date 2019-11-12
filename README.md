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
- http://meastp.github.io/cpp_kaffeprat/presentation.html?file=9.md
- http://meastp.github.io/cpp_kaffeprat/presentation.html?file=10.md

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
 - [ ] (9) utf-8 character literals
 - [ ] (9) splicing for maps and sets (insert_or_assign, try_emplace, merge, extract)
 - [ ] (9) inline variables
 - [ ] (9) std::optional
 - [ ] (9) std::any
 - [ ] (9) std::filesystem
 - [ ] (9) std::string_view
 
 - [ ] (10) std::variant, std::visit
 - [ ] (10) structured bindings
 - [ ] (10) selection statements (if og switch) with initializer
 - [ ] (10) std::apply, std::invoke
 - [ ] (10) fold expressions
 - [ ] (10) template argument deduction for class templates
 - [ ] (10) declaring non-type template parameters with auto
 - [ ] (10) if constexpr
 - [ ] (10) constexpr lambda
 - [ ] (10) lambda capture this by value

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
