## SOLID principles

#### S
<p>A class should have a single responsibility, if a Class has many responsibilities, it increases the possibility of bugs because making changes to one of its responsibilities, could affect the other ones without you knowing.
This principle aims to separate behaviours so that if bugs arise as a result of your change, it won’t affect other unrelated behaviours.</p>

#### O
*Open-Closed Principle*
<p>Classes should be open for extension, but closed for modification,  
software is made for solving a specific problem or meeting specific requirements in the real world and there is always a huge chance that the requirements will change.
Developers should take it with responsibility every time when we build any project, which includes the adoption of techniques that allows us to have a code structure that minimizes the chances to introduce new bugs in the cases when the business requirement changes.
</p>

#### L
*Liskov Substitution Principle*
<p>If S is a subtype of T, then objects of type T in a program may be replaced with objects of type S without altering any of the desirable properties of that program. 
If you have a Class and create another Class from it, it becomes a parent and the new Class becomes a child. The child Class should be able to do everything the parent Class can do. This process is called Inheritance.
The child Class should be able to process the same requests and deliver the same result as the parent Class or it could deliver a result that is of the same type.</p>

#### I
*Interface Segregation Principle*
<p>Clients should not be forced to depend on methods that they do not use. 
When a Class is required to perform actions that are not useful, it is wasteful and may produce unexpected bugs if the Class does not have the ability to perform those actions.</p>

#### D
*Dependency Inversion Principle*
<p>
  - High-level modules should not depend on low-level modules. Both should depend on the abstraction.
  - Abstractions should not depend on details. Details should depend on abstractions.</P>
