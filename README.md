# cpp_kaffeprat

# C++ Core Guidelines

https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines

# presentasjoner

- http://meastp.github.io/cpp_kaffeprat/1.html
- http://meastp.github.io/cpp_kaffeprat/2.html

# status

```cpp
using namespace std;
```
## C++11
 - [x] nullptr
 - [x] auto
 - [x] to_string
 - [x] tie, tuple
 - [x] array
 - [x] range-based for
 - [x] unique_ptr, make_unique
 - [x] shared_ptr, make_shared
 - [x] non-static data member initializers
 - [x] move semantics: move, forward, rvalue references og move constructors/-assignment
 - [x] default and deleted functions
 - [ ] std::mutex, std::recursive_mutex osv.
 - [ ] type traits (eks. std::is_integral<int>::value)
 - [ ] std::chrono
 - [ ] std::atomic
 - [ ] std::thread
 - [ ] std::future
 - [ ] std::lock, std::lock_guard
 - [ ] variadic templates
 - [ ] initializer lists
 - [ ] lambda-funksjoner
 - [ ] decltype
 - [ ] using (i stedet for typedef)
 - [ ] enum class ("strongly typed enums")
 - [ ] attributes
 - [ ] constexpr
 - [ ] delegating constructors
 - [ ] user-defined literals
 - [ ] override og final
 - [ ] inline-namespace

## C++14
 - [ ] binary literals
 - [ ] generic lambda expressions
 - [ ] lambda capture initializers
 - [ ] return type deduction
 - [ ] decltype(auto)
 - [ ] constexpr med færre begrensninger
 - [ ] variable templates
 - [ ] user-defined literals for standard library types
 - [ ] std::integer_sequence

## C++17
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
 - [ ] std::filesystem

## C++20 TBD
 - [ ] Concepts
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
 - [ ] Concepts (del av C++20)
 - [ ] Concurrency (v1 og v2)
 - [ ] Ranges
 - [ ] Coroutines
 - [ ] Networking
 - [ ] Modules
 - [ ] Reflection
 - [ ] Numerics
 - [ ] Graphics
 - [ ] Contracts
