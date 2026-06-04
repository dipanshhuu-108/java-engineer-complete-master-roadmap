# ADVANCED LANGUAGE CONSTRUCTS

## Packages
- Package Declaration
- Package Naming Convention
- Package Hierarchy
- Default Package
- Classpath
- Fully Qualified Name
- package-info.java

## Access Modifiers
- public
  - Accessible Everywhere
- private
  - Accessible Only Within Class
- protected
  - Accessible Within Package
  - Accessible in Subclasses
- Package-private (default, no modifier)
  - Accessible Within Package
- Summary Table
  - Class-level Modifiers
  - Member-level Modifiers

## Nested Classes
- Inner Classes
  - Non-static Inner Class
  - Enclosing Class Reference
  - this Reference Behavior
  - Instantiation of Inner Class
  - Access to Enclosing Class Members
  - Shadow References
- Static Nested Classes
  - Static Inner Class
  - No Reference to Enclosing Instance
  - Similar to Top-level Class
  - Instantiation
- Local Classes
  - Defined Inside Methods
  - Scope Limited to Method
  - Access to Local Variables
  - Effectively Final Variables
- Anonymous Classes
  - No Class Name
  - Defined Where Created
  - Implementing Interfaces
  - Extending Classes
  - Single Use Classes
  - Limitations

## Enum
- Enum Declaration
- Enum Constants
- Enum Variables
- Enum Methods
  - toString()
  - ordinal()
  - values()
  - valueOf()
- Enum with Constructor
- Enum with Fields
- Enum with Abstract Methods
- EnumSet
- EnumMap
- Enum Reflection
- Enum as Singleton

## Records (Java 14+, finalized in Java 16)
- Record Declaration
- Record Components
- Auto-generated Methods
  - constructor()
  - getter methods
  - equals()
  - hashCode()
  - toString()
- Compact Constructor
- Validation in Records
- Static Members in Records
- Custom Methods in Records
- Records vs Classes
- Records Serialization
- Records and Reflection

## Sealed Classes (Java 15+, finalized in Java 17)
- Sealed Class Declaration
- permits Clause
- Sealed Hierarchies
- Inheritance Restrictions
- Sealed + non-sealed
- final Subclasses
- Benefits of Sealed Classes
- Pattern Matching with Sealed Classes

## Pattern Matching
- Pattern Matching for instanceof (Java 16+)
  - Type Pattern
  - Type Narrowing
  - Pattern Variable
  - Scope of Pattern Variable
- Pattern Matching for switch (Java 17+, preview → 21 finalized)
  - Type Patterns
  - Value Patterns
  - Guarded Patterns
  - Parenthesized Patterns
  - Record Patterns (Java 19+, preview)

## instanceof Enhancements
- Traditional instanceof
- Pattern Matching instanceof (Java 16+)
- Type Pattern Binding
- Null Safety
- Instanceof Chain

## Text Blocks (Java 13+, finalized in Java 15)
- Text Block Syntax ("""...""")
- Multi-line Strings
- Escape Sequences
- Leading Whitespace Stripping
- Line Terminator Control
- Text Block Advantages
- Use Cases

## Switch Pattern Matching (Java 17+, preview → 21 finalized)
- Enhanced switch Expression
- Pattern Labels
- Guard Expressions
- Type Pattern Matching
- Record Pattern Matching
- Exhaustiveness Checking
- default Label

## Virtual Threads Syntax (Java 19+, preview → 21 finalized)
- Virtual Thread Creation
  - Thread.ofVirtual()
  - Structured Concurrency API
- Virtual Thread Basics
- Platform Threads vs Virtual Threads
- Syntax for Virtual Threads
- Virtual Thread Benefits

## Modules (Java 9+, JPMS)
- Module Declaration
  - module-info.java
  - module Name
  - requires Directive
  - exports Directive
  - opens Directive
  - uses Directive
  - provides Directive
- Module Types
  - Named Modules
  - Unnamed Module
  - Automatic Module
- Module Relationships
  - Module Dependency
  - Transitive Dependencies
  - Qualified Exports
  - Service Loader
- Module Resolution
  - Module Path
  - Class Path
  - Backward Compatibility

## JPMS (Java Platform Module System)
- Module System Overview
- Module Boundaries
- Encapsulation
- Reliability
- Performance
- Migration Strategies

## Annotations
- Annotation Declaration
- Built-in Annotations
  - @Override
  - @Deprecated
  - @SuppressWarnings
  - @FunctionalInterface
  - @SafeVarargs
  - @Native
  - @Repeatable
- Meta Annotations
  - @Retention
    - RetentionPolicy.SOURCE
    - RetentionPolicy.CLASS
    - RetentionPolicy.RUNTIME
  - @Target
    - ElementType.TYPE
    - ElementType.METHOD
    - ElementType.FIELD
    - ElementType.PARAMETER
    - ElementType.CONSTRUCTOR
    - ElementType.LOCAL_VARIABLE
    - ElementType.ANNOTATION_TYPE
    - ElementType.PACKAGE
    - ElementType.TYPE_PARAMETER (Java 8+)
    - ElementType.TYPE_USE (Java 8+)
  - @Documented
  - @Inherited
  - @Repeatable (Java 8+)
- Repeatable Annotations
  - @Repeatable Meta-annotation
  - Containing Annotation
  - Accessing Repeated Annotations
- Custom Annotations
  - Annotation Elements
  - Element Types
  - Default Values
  - Marker Annotations
  - Single-Element Annotations
  - Multi-Element Annotations
- Annotation Processing
  - Retention Policies
  - Compile-time Processing
  - Runtime Processing
  - Reflection for Annotations

## Reflection Basics
- Class Object
  - forName()
  - getClass()
  - .class Literal
- Inspecting Classes
  - getName()
  - getSimpleName()
  - getSuperclass()
  - getInterfaces()
  - getModifiers()
- Inspecting Members
  - getMethods()
  - getDeclaredMethods()
  - getConstructors()
  - getDeclaredConstructors()
  - getFields()
  - getDeclaredFields()
- Accessing Method Information
  - Method Name
  - Return Type
  - Parameter Types
  - Exceptions
  - Modifiers
- Invoking Methods Reflectively
  - Method.invoke()
  - Parameter Passing
  - Return Value
  - Exception Handling
- Creating Instances Reflectively
  - Constructor.newInstance()
  - Array Creation
  - No-arg Constructor
- Accessing Fields Reflectively
  - Field.get()
  - Field.set()
  - Primitive Field Handling
  - setAccessible(true)
- Annotation Reflection
  - getAnnotations()
  - getAnnotation()
  - getDeclaredAnnotations()
- Type Parameters and Generics
  - getTypeParameters()
  - getGenericSuperclass()
  - Type Erasure Limitations
