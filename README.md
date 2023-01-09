# Class Notes Week 2
## UML Example
<img width="784" alt="Screen Shot 2022-09-09 at 9 21 10 PM" src="https://user-images.githubusercontent.com/102199778/189465181-22f7b753-8848-4094-b9ce-172772563abf.png">
UML is a spatial representation that cescribes: definition of a class and how different classes relate

- neg = private

- pos = public 

- underlined = static

- all caps = final var

## Problem Solving
- understand the problem
- design a solution
- consider alternatives and refine
- impliment the solution
- test the solution

## Java Objects
**Class:** a means of creating new types
- group data elements that describe an abstract concept

#### An object is one instance of a class
- occupies a block of memory in the heap that contains the values of the data elements
- each instance has its own memory
- the set of values stored in this memory block is called the state of the object
- in code we refer to object instances using a reference to the memory block

<img width="414" alt="Screen Shot 2022-09-09 at 9 51 52 PM" src="https://user-images.githubusercontent.com/102199778/189466042-cda75cdd-125a-4cca-b410-25807dfa4c22.png">

## Instance Methods
- Accessors: Methods used to report the stat of objects
- Mutators: Methods used to change the state of objects

## Instance Methods: Special Cases
- Getters: Accessor methods used to report the low-level state of objects
- Setters: Mutator methods used to change the low-level state of objects
#### Mutator methods: 
- if there are no methods that change the state of an object. These are called immutable classes
- there may be many methods that change the object's state. We call these classes mutable

## A Class is a Contract
the set of instance methods define the legal ways that an object may be accessed/changed
- all operations on an object: must always leave the object in a consistent state
- Best practice: On entry assume the object is in a constant state. On exit, ensure that it is still consistent

## A Class as an "Encapsulator"
- classes hide details from the user
- user only interacts with the class' public interface

## Public vs Private Data
#### Public pros
- easy access to all data by other classes
- don't need getters and setters
#### Public cons
- can't protect the data from other classes

#### For this class:
- we want to protect themselves; therefore instance variables will be private/protected

## Instance vs Class Data
- each object gets its own copy of instance data
- all objects in a class share one copy of class data
  - static variables
  
## Class Variables
Only one copy of the variables for all instances in the class
- declare as static

## Class Methods
- many have no access to instance data
  - there is no object so no instance variables

## Method Overloading
**Overloading:** using the same method name but different parameters and/or return type

## this.
- this. references the class variable with the name 
- As constructor
<img width="350" alt="Screen Shot 2022-09-09 at 10 10 50 PM" src="https://user-images.githubusercontent.com/102199778/189466541-b141ab44-227b-4eb6-a908-1b41c04acc08.png">


## Classes within classes
- define classes hierarchically = W
- Once “Player”, able to create new classes with Player
<img width="471" alt="Screen Shot 2022-09-09 at 10 12 39 PM" src="https://user-images.githubusercontent.com/102199778/189466590-b3511e5d-c98c-4482-8770-9a814d28bd12.png">

- constructors can use the default constructor to handle some initialization

## File Handling
<img width="619" alt="Screen Shot 2022-09-08 at 3 00 27 PM" src="https://user-images.githubusercontent.com/102199778/189214726-9c34fd9d-b0e3-4f7d-aac3-136d05c2563b.png">
