Polymorphism in C++
===================

There are four major ways to get polymorphism behavior in C++.

* **Template** (Compile-time polymorphism)
* **Virtul function** (Run-time polymorphism)

## How the Compiler Processes Templates

When the compiler encounters an intantiation of the template, such as `Grid<int> myGrid`, it writes the code for an `int` version of the `Grid` template by replacing each `T` in the template class definition with `int`.

If you don't intantiate a class template for any types in your program, then the class method definitions are never compiled.

### Selective intantiation

The compiler generates code only for the class methods that you actually call for a particular type.