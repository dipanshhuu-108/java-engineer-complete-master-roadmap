# OBJECT ORIENTED PROGRAMMING

## Classes
- Class Declaration
- Class Modifiers (public, final, abstract)
- Class Members
  - Variables (Fields)
  - Methods
  - Constructors
  - Initializers
  - Inner Classes
- Class Definition
- Object Creation

## Objects
- Object Instantiation
- Object References
- Object Identity
- Object State
- Object Behavior
- Garbage Collection

## Constructors
- Default Constructor
  - Implicit Default Constructor
  - Explicit Default Constructor
- Parameterized Constructor
  - Parameter Passing
  - Field Initialization
- Constructor Chaining
  - this() Call
  - super() Call
  - Constructor Delegation
- Copy Constructor Pattern
  - Shallow Copy
  - Deep Copy

## Keywords
- this Keyword
  - Instance Variable Reference
  - Method Invocation
  - Constructor Chaining
  - Return this
- super Keyword
  - Parent Class Reference
  - super() Constructor Call
  - super.method() Invocation
  - super.field Access
- static Keyword
  - Static Variables
  - Static Methods
  - Static Initializer Blocks
  - Static Context Limitations
  - Static Import
- final Keyword
  - final Class
  - final Method
  - final Variable
  - final Parameter
  - final Object Reference
- transient Keyword
  - Serialization Exclusion
  - Transient Fields
- volatile Keyword
  - Memory Visibility
  - Visibility Guarantee
  - Not a Lock
  - Use Cases
- synchronized Keyword
  - Synchronized Methods
  - Synchronized Blocks
  - Intrinsic Locks
- native Keyword
  - JNI (Java Native Interface)
  - Native Methods
  - Platform-specific Code
- strictfp Keyword
  - Strict Floating-point
  - Precision Guarantee
- abstract Keyword
  - Abstract Classes
  - Abstract Methods
  - Cannot Instantiate

## Pillars of OOP
- Encapsulation
  - Data Hiding
  - Getter and Setter Methods
  - Access Modifiers
  - Information Hiding
- Inheritance
  - IS-A Relationship
  - Parent Class
  - Child Class
  - Single Inheritance
  - Multi-level Inheritance
  - Method Overriding
  - super Keyword
- Polymorphism
  - Compile-time Polymorphism (Method Overloading)
  - Runtime Polymorphism (Method Overriding)
  - Dynamic Method Dispatch
  - Polymorphic References
  - Liskov Substitution Principle
- Abstraction
  - Abstract Classes
  - Interfaces
  - Abstract Methods
  - Hiding Implementation Details
  - Abstraction vs Encapsulation

## Object Relationships
- IS-A Relationship
  - Inheritance
  - Parent-Child Hierarchy
- HAS-A Relationship
  - Composition
  - Aggregation
  - Object Containment
- Association
  - One-to-One
  - One-to-Many
  - Many-to-One
  - Many-to-Many
- Aggregation
  - Weak Association
  - Part-Whole Relationship
  - Can Exist Independently
  - Shared Ownership
- Composition
  - Strong Association
  - Part-Whole Relationship
  - Cannot Exist Independently
  - Exclusive Ownership

## Interfaces
- Interface Declaration
- Interface Members
  - Abstract Methods
  - Constants
  - Default Methods (Java 8+)
  - Static Methods (Java 8+)
  - Private Methods (Java 9+)
  - Private Static Methods (Java 9+)
- Interface Implementation
  - implements Keyword
  - Multiple Interface Implementation
  - Interface Inheritance
- Default Methods
  - Method Implementation in Interface
  - Backward Compatibility
  - Diamond Problem Resolution
  - super.methodName() Call
- Static Methods
  - Interface Static Methods
  - Called via Interface Name
  - Cannot Be Overridden
- Functional Interfaces
  - Single Abstract Method (SAM)
  - @FunctionalInterface Annotation
  - Lambda Expression Support
- Marker Interfaces
  - No Methods or Constants
  - Serializable Interface
  - Cloneable Interface
  - RandomAccess Interface
  - Purpose: Tagging

## Abstract Classes
- Abstract Class Declaration
- Abstract Methods
  - Method Declaration Without Body
  - Must Be Overridden
- Concrete Methods in Abstract Classes
- Abstract Class Instantiation (Cannot)
- Abstract Class Inheritance
- Abstract vs Interface
- When to Use Abstract Classes

## Object Class
- Object Class Hierarchy
- Methods in Object Class
  - equals()
  - hashCode()
  - toString()
  - clone()
  - getClass()
  - finalize()
  - wait(), notify(), notifyAll()
  - Deprecated Methods (wait, notify variants)

## equals() Method
- Default Implementation
- Overriding equals()
- equals() Contract
  - Reflexive
  - Symmetric
  - Transitive
  - Consistent
  - Null Safety
- equals() vs ==
- equals() Implementation Patterns

## hashCode() Method
- Default Implementation
- Overriding hashCode()
- hashCode() Contract
  - Consistency
  - equals() Consistency
- hashCode() Implementation
- Hash Function Design
- Immutable hashCode()

## clone() Method
- Default Implementation (Shallow Copy)
- Cloneable Interface
- Overriding clone()
- Shallow Copy vs Deep Copy
- CloneNotSupportedException
- Copy Constructor Alternative
- Clone Performance

## toString() Method
- Default Implementation
- Overriding toString()
- toString() Convention
- Useful toString() Implementation

## finalize() Method
- Finalization
- finalize() Purpose
- Garbage Collection Trigger
- Deprecated (Java 9+)
- finalize() Alternative (try-with-resources, Cleaner API)

## Immutability
- Immutable Objects
- Creating Immutable Classes
  - final Class
  - final Fields
  - Private Constructor
  - No Setters
  - Defensive Copying
- Immutable Collection Wrappers
- Benefits of Immutability
  - Thread Safety
  - Caching
  - String Interning
  - Value Objects

## Object Modeling
- Domain Objects
- Value Objects
- Entity Objects
- Service Objects
- DTO (Data Transfer Objects)
- POJO (Plain Old Java Objects)
- Bean Class Conventions
  - No-arg Constructor
  - Getter and Setter Methods
  - Serializable
