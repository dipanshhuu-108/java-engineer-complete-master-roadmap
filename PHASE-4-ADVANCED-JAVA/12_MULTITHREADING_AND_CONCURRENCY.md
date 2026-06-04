# MULTITHREADING AND CONCURRENCY

## Thread Lifecycle
- Thread States
- Thread Creation
- Thread Starting
- Thread Execution
- Thread Termination

## Runnable
- Runnable Interface
- Implementing Runnable
- Anonymous Runnable
- Lambda Runnable (Java 8+)

## Callable
- Callable Interface
- Callable vs Runnable
- Implementing Callable

## Future
- Future Interface
- Future Operations
- Exception Handling
- Future Composition

## CompletableFuture
- CompletableFuture Concept (Java 8+)
- Creating CompletableFuture
- Completing CompletableFuture
- Transforming Results
- Combining Multiple Futures
- Error Handling
- Async Continuation
- CompletableFuture Best Practices

## Executor Framework
- Executor Interface
- ExecutorService Interface
- Thread Pool Executors
- ThreadPoolExecutor
- Executor Lifecycle
- Task Submission
- Work Queues
- Rejection Policies

## ForkJoinPool
- ForkJoinPool Concept
- ForkJoinPool Creation
- ForkJoinTask Submission
- Work Stealing Algorithm
- Monitoring

## Synchronization
- Synchronization Need
- Critical Section

## Monitors
- Monitor Concept
- Monitor Lock

## Intrinsic Locks
- Object Intrinsic Lock
- synchronized Method
- Lock Acquisition
- Lock Release
- Lock Reentrancy

## ReentrantLock
- ReentrantLock Class
- ReentrantLock Methods
- Fair Lock
- Condition
- ReentrantLock vs synchronized

## ReadWriteLock
- ReadWriteLock Concept
- ReentrantReadWriteLock
- Read Lock
- Write Lock
- Lock Upgrade/Downgrade

## StampedLock
- StampedLock Concept (Java 8+)
- StampedLock Methods
- Optimistic Read
- Regular Read Lock
- Write Lock
- Lock Conversion

## Semaphore
- Semaphore Concept
- Creating Semaphore
- Semaphore Operations
- Binary Semaphore
- Counting Semaphore
- Semaphore Use Cases

## CountDownLatch
- CountDownLatch Concept
- Creating CountDownLatch
- CountDownLatch Operations
- One-shot Usage
- CountDownLatch Use Cases

## CyclicBarrier
- CyclicBarrier Concept
- Creating CyclicBarrier
- CyclicBarrier Operations
- Reusable Barrier
- Barrier Action
- CyclicBarrier Use Cases

## Phaser
- Phaser Concept (Java 7+)
- Creating Phaser
- Phaser Operations
- Phaser Advance
- Phaser Use Cases

## Exchanger
- Exchanger Concept
- Creating Exchanger
- Exchanger Operations
- Blocking Semantics
- Exchanger Use Cases

## Atomic Classes
- Atomic Variable Concept
- AtomicInteger
- AtomicLong
- AtomicReference<V>
- AtomicBoolean
- Atomic Arrays
- Atomic Field Updaters
- Lock-free Algorithms

## CAS (Compare-and-Swap)
- CAS Operation
- CAS Implementation
- CAS Limitations
- ABA Problem
- CAS Performance

## Volatile
- volatile Keyword
- Visibility Guarantee
- Memory Barrier
- volatile Use Cases
- volatile vs Synchronization

## ThreadLocal
- ThreadLocal Concept
- Creating ThreadLocal
- ThreadLocal Operations
- ThreadLocal Use Cases
- Memory Leak Risk
- InheritableThreadLocal

## Concurrent Collections
- ConcurrentHashMap
- ConcurrentSkipListMap
- CopyOnWriteArrayList
- CopyOnWriteArraySet
- BlockingQueue
- ConcurrentLinkedQueue
- Concurrent Collection Semantics

## Java Memory Model
- JMM Concept
- Actions in JMM
- Ordering Rules
- Memory Barriers

## Happens-Before
- Happens-before Relationship
- Happens-before Rules
- Data Race Freedom

## Deadlock
- Deadlock Concept
- Deadlock Conditions
- Deadlock Prevention
- Deadlock Avoidance
- Deadlock Recovery
- Lock Ordering

## Livelock
- Livelock Concept
- Livelock vs Deadlock
- Livelock Causes
- Livelock Prevention

## Starvation
- Starvation Concept
- Causes
- Starvation Prevention

## Race Conditions
- Race Condition Concept
- Race Condition Types
- Check-then-act
- Race Condition Prevention

## False Sharing
- False Sharing Concept
- Cache Line
- False Sharing Examples
- False Sharing Prevention

## Virtual Threads
- Virtual Thread Concept (Java 19+)
- Creating Virtual Threads
- Virtual Thread Characteristics
- Virtual Thread Limitations
- Virtual Thread Use Cases
- Virtual vs Platform Threads

## Structured Concurrency
- Structured Concurrency Concept (Java 19+, Preview)
- StructuredTaskScope
- Task Outcome
- Structured Concurrency Benefits

## Concurrency Design Patterns
- Producer-Consumer
- Reader-Writer Lock
- Thread Pool
- Barrier Synchronization
- Latch
- Future
- Thread Confinement
- Immutability
