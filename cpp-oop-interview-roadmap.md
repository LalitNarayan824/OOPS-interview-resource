# C++ OOP Interview Preparation Roadmap

A structured checklist to cover Object-Oriented Programming in C++ for interviews.

---

## 1. Core Pillars
- [ ] What is OOP? Why use it over procedural programming?
- [ ] Explain **Encapsulation**, **Abstraction**, **Inheritance**, **Polymorphism** with real examples
- [ ] Difference between Abstraction and Encapsulation

## 2. Classes & Objects
- [ ] Difference between `struct` and `class` in C++
- [ ] Access specifiers (`public`, `private`, `protected`) and their behavior in inheritance
- [ ] What is the `this` pointer? Can it be `nullptr`?
- [ ] Static members vs instance members — storage, and can a static function access non-static members?

## 3. Constructors & Destructors
- [ ] Types: default, parameterized, copy constructor, delegating constructor
- [ ] When is a copy constructor called? Shallow vs deep copy
- [ ] The `explicit` keyword — why use it?
- [ ] Rule of Three / Rule of Five / Rule of Zero
- [ ] Order of constructor/destructor calls in inheritance
- [ ] Why should base class destructors be `virtual`? What happens if they aren't?
- [ ] Can a constructor be virtual? Why not?
- [ ] Calling a virtual function from a constructor/destructor — what happens?

## 4. Inheritance
- [ ] Types: single, multiple, multilevel, hierarchical, hybrid
- [ ] The **diamond problem** and how `virtual` inheritance solves it
- [ ] Difference between `public`, `private`, `protected` inheritance
- [ ] **Object slicing** — what it is and how to avoid it
- [ ] Composition vs Aggregation vs Inheritance ("has-a" vs "is-a")

## 5. Polymorphism
- [ ] Compile-time (overloading, operator overloading, templates) vs Runtime (virtual functions)
- [ ] How **vtable/vptr** works internally
- [ ] Function overloading vs overriding vs hiding
- [ ] Pure virtual functions and abstract classes
- [ ] Can an abstract class have a constructor? Can it be instantiated?
- [ ] Early binding vs late binding
- [ ] Covariant return types
- [ ] `final` and `override` keywords

## 6. Operator Overloading & Friend
- [ ] Rules for overloading operators; which ones can't be overloaded (`::`, `.`, `.*`, `?:`, `sizeof`)
- [ ] Why overload `<<` / `>>` as friend functions, not members
- [ ] What is a friend function/class? Does it break encapsulation?

## 7. Memory & Modern C++ Tie-ins
- [ ] Deep copy vs shallow copy — implement a proper copy constructor
- [ ] Move constructor / move assignment, `std::move`
- [ ] Smart pointers (`unique_ptr`, `shared_ptr`) and RAII in OOP context
- [ ] Multiple inheritance and memory layout issues

## 8. Design-Oriented (Mid/Senior Level)
- [ ] SOLID principles with C++ examples (especially LSP and OCP)
- [ ] Interfaces in C++ (pure abstract classes) — simulating Java-style interfaces
- [ ] Inheritance vs interfaces vs templates (static polymorphism) — when to use which

## 9. Practical / Coding Round Prep
- [ ] Implement a class demonstrating Rule of Five
- [ ] Overload operators for a `Complex` number or `Matrix` class
- [ ] Design a class hierarchy (e.g., `Shape -> Circle, Rectangle`) using pure virtual functions
- [ ] Fix a "memory leak" snippet caused by a non-virtual base destructor
- [ ] Trace output of code involving virtual functions and constructor/destructor order

---

### Prep Tip
For each topic, write a small C++ snippet yourself and predict the output before running it — especially for:
- Constructor/destructor order
- Virtual function dispatch
- Object slicing

Interviewers frequently give "predict the output" code snippets exactly on these three areas.
