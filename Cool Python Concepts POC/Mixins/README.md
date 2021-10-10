## Mixins in Python

1. It is an alternative class design pattern.
2. It has an edge over single inheritance and multiple inheritance.
3. There is the problem of forming long chains A -> B -> C -> D -> E in Single Inheritance and problem of code dirtiness/ unclear and messy codes in Multiple inheritance.
4. Mixin architecture is a good way to make code clean and reduce redundancy.
5. It is pretty easy to implement.
6. Example: -

![Mixins Diagram](D:\DATA SCIENCE\GitHub\Cool Python Concepts with POC\Mixins\diagram.drawio)


Here,
- class A has a variable total.
- class B and C inherits A.
- D inherits B and E inherits C.
- Our requirement iss to introduce a function in both D and E that prints total.
- So we have got no other choice but to write code snippets in both D and E individually.
- These are just 2 classes where redundancy is happening. Imagine the case where print_total() functionality is desireable in 20 classes.
- The code will look so messy if we start introducing print_total() in all the 20 classes.
- Mixins solve this! 
- We create a Mixin class.
- A mixin is a class that defines and implements a single, well-defined feature. Sub-classes that inherit from mixin class, inherit just this feature and nothing else.


#### Implementation
We create the classes, A, B, C, D, E and M (Mixin class).

Mixin class with have the functionality print_total(). Classes D and E inherit M and therefore inherit print_total(). We need not re-write the code again and again.

See the python files attached.


