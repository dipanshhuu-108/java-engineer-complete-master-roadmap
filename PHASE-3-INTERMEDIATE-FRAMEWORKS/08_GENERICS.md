# GENERICS

## Generic Classes
- Generic Class Declaration
  - <T> Syntax
  - Type Parameter
- Generic Class Usage
  - Instantiation with Type Argument
  - Type Safety
  - Generic Type Reference
- Multiple Type Parameters
  - <T, U, V>
  - Independent Type Parameters
- Nested Generics
  - List<List<String>>
  - Nested Type Parameters

## Generic Interfaces
- Generic Interface Declaration
  - <T> in Interface
- Implementing Generic Interface
  - Type Parameter in Implementation
  - Concrete Type Implementation
- Generic Interface Usage
- Extending Generic Interface
  - Adding Type Parameters
  - Type Parameter Propagation

## Generic Methods
- Generic Method Declaration
  - <T> Before Return Type
- Generic Method Invocation
  - Explicit Type Argument
  - Type Inference
  - Diamond Operator
- Type Inference in Methods
- Multiple Type Parameters in Methods
- Static Generic Methods
- Generic Method Override

## Type Parameters
- Type Variable Declaration
  - Naming Convention (T, U, V, E, K, V, N)
  - Single Letter Names
- Type Parameter Scope
  - Class Scope
  - Method Scope
- Type Parameter Substitution
  - Actual Type Argument
  - Binding
  - Type Erasure

## Bounded Types
- Upper Bounded Wildcard
  - <? extends T>
  - Subtype of T
  - Read-only Constraint
  - Use Cases
- Lower Bounded Wildcard
  - <? super T>
  - Supertype of T
  - Write-capable
  - Use Cases
- Unbounded Wildcard
  - <?>
  - Any Type
  - Limited Operations
- Type Variable Bounds
  - <T extends Class>
  - <T extends Interface>
  - Single Upper Bound
- Multiple Bounds
  - <T extends Class & Interface>
  - First Bound Must Be Class
  - Multiple Interface Bounds

## Multiple Bounds
- Single Type Variable with Multiple Bounds
  - <T extends Base & Interface1 & Interface2>
- Type Parameter Ordering
  - Class Bound First
  - Interface Bounds After
- Constraint Satisfying
  - Type Must Satisfy All Bounds

## Wildcards
- Unbounded Wildcard
  - <?>
  - Most Permissive
  - Limited Utility
- Bounded Wildcard (Upper)
  - <? extends T>
  - More Specific
  - Read-only
  - Covariance
- Bounded Wildcard (Lower)
  - <? super T>
  - Contravariance
  - Write-capable
  - PECS (Producer Extends, Consumer Super)
- Wildcard Capture
  - Type Variable Capture
  - Helper Methods
  - Capturing Type Information

## Covariance
- Covariant Type
  - <? extends T>
  - Subtypes Substitutable
  - Read-only Use
  - Producer Pattern
  - Example: List<? extends Number>
    - Can Read as Number
    - Cannot Write Specific Subtype

## Contravariance
- Contravariant Type
  - <? super T>
  - Supertypes Substitutable
  - Write-capable
  - Consumer Pattern
  - Example: List<? super Integer>
    - Can Write Integer
    - Can Read as Object

## PECS (Producer Extends, Consumer Super)
- Producer Pattern
  - Use <? extends T>
  - When Reading from Generic
  - Maximize Flexibility for Reading
- Consumer Pattern
  - Use <? super T>
  - When Writing to Generic
  - Maximize Flexibility for Writing
- Choosing Between Extends/Super
  - Extend for Reading
  - Super for Writing
  - None if Both

## Type Erasure
- Erasure Process
  - Generic Information Removed at Runtime
  - Type Parameters Replaced with Bounds
  - Replaced with Object if No Bound
  - Backward Compatibility
- Implications
  - No Runtime Type Information
  - Cannot Use Primitive Types
  - Cannot Create Generic Array Directly
  - Cannot Use instanceof with Generic Types
  - Cannot Instantiate Type Parameters
- Type Erasure Examples
  - List<String> → List
  - <T extends Number> → Number
  - <T> → Object
- Erasure Consequences
  - Generic and Non-generic Coexistence
  - Type Safety at Compile Time
  - Runtime Limitations

## Bridge Methods
- Bridge Method Generation
  - Compiler-generated Methods
  - Type Erasure Workaround
  - Method Override with Different Erasure
- Bridge Method Example
  - Generic Method Override
  - Synthetic Bridge Method
  - Reflection Detection
  - isBridge() on Method

## Generic Design Patterns
- Generic Factory Pattern
  - Generic Factory Method
  - Type-safe Object Creation
- Generic Singleton Pattern
  - Type-safe Singleton
  - Static Holder
- Generic Builder Pattern
  - Fluent API with Generics
  - Type Safety
  - Complex Object Construction
- Type Token Pattern
  - Class<T> as Type Token
  - Runtime Type Information
  - Generic Type Capture
- Recursive Type Bound
  - <T extends Comparable<T>>
  - Self-referential Bound
  - Type Safety for Comparable
