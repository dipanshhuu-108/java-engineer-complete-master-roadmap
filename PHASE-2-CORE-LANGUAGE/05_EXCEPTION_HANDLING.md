# EXCEPTION HANDLING

## Exception Hierarchy
- Throwable (Root)
  - Error
    - VirtualMachineError
    - OutOfMemoryError
    - StackOverflowError
    - ExceptionInInitializerError
  - Exception
    - Checked Exception
    - Unchecked Exception (RuntimeException)

## Error
- Error Type
- Non-recoverable Errors
- System-level Errors
- Application Should Not Catch
- Examples
  - OutOfMemoryError
  - StackOverflowError
  - VirtualMachineError

## Exception
- Exception Type
- Recoverable Errors
- Application-level Exceptions
- Exception Hierarchy

## Checked Exceptions
- Definition
- Compile-time Checking
- Must Be Caught or Declared
- throws Declaration
- Common Checked Exceptions
  - IOException
  - SQLException
  - ClassNotFoundException
  - InterruptedException
  - ReflectiveOperationException

## Unchecked Exceptions (RuntimeException)
- Definition
- No Compile-time Checking
- Can Be Caught (Optional)
- Common Unchecked Exceptions
  - NullPointerException
  - ArrayIndexOutOfBoundsException
  - ClassCastException
  - IllegalArgumentException
  - IllegalStateException
  - ArithmeticException
  - NumberFormatException
  - UnsupportedOperationException

## try Block
- try Syntax
- Resource Allocation
- Exception May Occur
- Block Execution
- Multiple Statements

## catch Block
- catch Clause
- Exception Parameter
- Exception Variable Scope
- Multiple catch Blocks
- Order of catch Blocks
- Exception Handling
- Re-throwing

## finally Block
- finally Clause
- Guaranteed Execution
- Cleanup Operations
- finally Without catch
- Return Statement in finally
- Exception in finally
- finally Execution Guarantee

## throw Statement
- throw Syntax
- Throwing Exceptions
- Creating Exception Objects
- Propagating Exceptions
- Throwing Custom Exceptions
- Exception Message

## throws Clause
- throws Declaration
- Method Signature
- Propagating Checked Exceptions
- Multiple Exceptions
- Exception Declaration Order
- Method Override throws Clause

## Multi Catch
- Multi-catch Syntax (Java 7+)
- Pipe Operator (|)
- Multiple Exception Types
- Catching Multiple Exceptions in One Block
- Exception Variable Type
- Catching Exception Hierarchy

## Nested Exceptions
- Nested try-catch
- Inner Exception Handling
- Outer Exception Handling
- Exception Propagation
- Multi-level Exception Handling

## Chained Exceptions
- Exception Cause
- initCause()
- Constructor with Cause Parameter
- getCause()
- Stack Trace with Chain
- Preserving Original Exception

## Suppressed Exceptions
- Suppressed Exception Concept
- addSuppressed()
- getSuppressed()
- try-with-resources Suppression
- Multiple Suppressed Exceptions
- Accessing Suppressed List

## Try With Resources
- try-with-resources Syntax (Java 7+)
- AutoCloseable Interface
- Automatic Resource Closing
- Multiple Resources
- Resource Variable Scope
- Suppressed Exceptions
- Enhanced try-with-resources (Java 9+)

## AutoCloseable Interface
- AutoCloseable Contract
- close() Method
- Exception Handling in close()
- try-with-resources Usage
- Implementing AutoCloseable
- Resource Management

## Custom Exceptions
- Creating Custom Exception Classes
- Extending Exception
- Extending RuntimeException
- Custom Exception Constructor
- Exception Message
- Exception Documentation
- When to Create Custom Exceptions

## Exception Design Strategies
- Exception Hierarchy Design
- Checked vs Unchecked
- Exception Wrapping
- Exception Transformation
- Exception Abstraction
- Exception Translation
- Fail-fast Principle
- Exception Cause Preservation
