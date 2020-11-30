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
- http://meastp.github.io/cpp_kaffeprat/presentation.html?file=11.md
- http://meastp.github.io/cpp_kaffeprat/presentation.html?file=12.md

# status

```cpp
using namespace std;
```
## [C++11](https://en.cppreference.com/w/cpp/11)
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

## [C++14](https://en.cppreference.com/w/cpp/14)
 - [x] (8) constexpr med færre begrensninger
 - [x] (8) user-defined literals for standard library types
 - [x] (8) binary literals
 - [x] (8) lambda capture initializers
 - [x] (8) generic lambda expressions
 - [x] (8) return type deduction
 - [x] (8) decltype(auto)
 - [x] (8) std::integer_sequence
 - [x] (8) variable templates

## [C++17](https://en.cppreference.com/w/cpp/17)
 - [x] (9) nested namespaces
 - [x] (9) utf-8 character literals
 - [x] (9) splicing for maps and sets (insert_or_assign, try_emplace, merge, extract)
 - [x] (9) inline variables
 - [x] (9) std::optional
 - [x] (9) std::any
 - [x] (9) std::filesystem
 - [x] (9) std::string_view
 
 - [x] (10) std::variant, std::visit
 - [x] (10) structured bindings
 - [x] (10) selection statements (if og switch) with initializer
 - [x] (10) std::apply, std::invoke
 - [x] (10) fold expressions
 - [x] (10) template argument deduction for class templates
 - [x] (10) declaring non-type template parameters with auto
 - [x] (10) if constexpr
 - [x] (10) constexpr lambda
 - [x] (10) lambda capture this by value

## [C++20](https://en.cppreference.com/w/cpp/20)
 - [x] (11) range-based for with initializer
 - [x] (11) `std::starts_with` `std::ends_with` for `std::string` og `std::string_view`
 - [x] (11) uniform container erasure (`std::erase` og `std::erase_if`)
 - [x] (11) `std::u8string`
 - [x] (11) `std::bind_front`
 - [x] (11) `std::endian`
 - [x] (11) `<numbers>` - matematiske konstanter
 - [x] (11) `std::jthread` - joining thread with cancellation
 - [x] (11) `<source_location>`
 - [x] (11) `<span>`
 - [ ] (12) `<bit>`
 - [ ] (12) consteval, constinit
 - [ ] (12) mer constexpr (`std::vector` `std::string`)
 - [ ] (12) designated initializers (fra C)
 - [ ] (12) 3-way comparison `<=>` og `operator==() = default` og `<compare>`
 - [ ] `<format>`
 - [ ] Calendar and Time Zone library (`<chrono>`)
 - [ ] abbreviated function templates
 - [ ] `<concepts>`
 - [ ] `<coroutine>`
 - [ ] modules
 - [ ] `<ranges>`

## C++23 TBD
 - [ ] stacktrace
 - [ ] `string::contains`
 - [ ] `size_t` -> `100uz`
 - pattern matching?
 - modules for std?
 - coroutine task?

## Oppsummering Unicode
