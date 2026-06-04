# JVM DEEP DIVE

## Class Loading
- Class Loading Process
- Loading Phase
- Linking Phase
- Initialization Phase
- Class Loading Sequence

## Class Loader Hierarchy
- Bootstrap Class Loader
- Extension Class Loader
- Application Class Loader
- Custom Class Loaders
- Hierarchy Structure

## Delegation Model
- Delegation Principle
- Upward Delegation
- Circular Loading Prevention
- Class Uniqueness

## Runtime Data Areas
- Method Area
  - Class Structures
  - Method Data
  - Code
  - Constants
- Heap
  - Shared Among All Threads
  - Garbage Collection
  - Size Configuration
- Stack (JVM Stack)
  - Per-thread
  - Stack Frames
  - Stack Overflow
- Program Counter (PC) Register
  - Current Instruction
  - Per-thread
  - Native Method Tracking
- Native Method Stack
  - Native Code
  - JNI Calls
  - Implementation Dependent

## Heap
- Heap Concept
- Heap Size Configuration
- Xmx, Xms Parameters
- Garbage Collection Regions
- Object Allocation

## Stack
- JVM Stack Structure
- Stack Frames
- Local Variables Array
- Operand Stack
- Method Invocation
- Stack Overflow

## Metaspace
- Metaspace (Java 8+)
- Replacing PermGen
- Native Memory
- Automatic Sizing
- Configuration

## Native Memory
- Off-heap Memory
- Direct Memory
- ByteBuffer Allocation
- Memory Mapping
- Native Code Allocation

## Garbage Collection
- Garbage Collection Concept
- Mark-Sweep
- Mark-Sweep-Compact
- Copying Algorithm
- Generational Hypothesis

## GC Algorithms
- Serial GC
- Parallel GC (ParNew, Parallel Scavenge)
- Concurrent Mark Sweep (CMS)
- G1 Garbage Collector
- Z Garbage Collector (ZGC)
- Shenandoah

## Serial GC
- Single-threaded Collection
- Stop-the-world Pauses
- Young Generation
- Old Generation
- Client JVM Default

## Parallel GC
- Multi-threaded Collection
- Parallel Young Generation
- Parallel Old Generation
- Throughput Focused
- Server JVM Default

## CMS
- Concurrent Mark Sweep
- Concurrent Marking
- Concurrent Sweeping
- Low Pause Time
- Fragmentation Issues

## G1
- Garbage First
- Regions
- Young Generation
- Old Generation
- Mixed Collections
- Predictable Pause Time

## ZGC
- Z Garbage Collector
- Concurrent
- Ultra-low Pause Time
- Colored Pointers
- Load Barriers

## Shenandoah
- Concurrent GC
- Concurrent Compaction
- Brooks Pointers
- Ultra-low Pause Time
- Concurrent Evacuation

## JIT
- Just-In-Time Compilation
- Bytecode to Native Code
- Performance Improvement
- Warm-up Period

## C1 Compiler
- Client Compiler
- Fast Compilation
- Lower Optimization
- Quick Startup

## C2 Compiler
- Server Compiler
- Aggressive Optimization
- Longer Compilation Time
- Better Performance

## Tiered Compilation
- C1 + C2 Combined
- Quick Startup + Good Performance
- Profiling
- Method Optimization

## Compilation Thresholds
- Invocation Count
- Branch Count
- Threshold Configuration
- Compilation Triggers

## Escape Analysis
- Object Escape
- Scalar Replacement
- Stack Allocation
- Synchronization Elimination
- Lock Elision

## Heap Dumps
- Heap Dump Generation
- jmap Tool
- Analysis Tools
- Memory Leak Detection

## Thread Dumps
- Thread Dump Generation
- jstack Tool
- Thread State Analysis
- Deadlock Detection

## JFR
- Java Flight Recorder
- Event Recording
- Low Overhead
- Production Profiling

## JMC
- Java Mission Control
- JFR Analysis
- Performance Monitoring
- Real-time Metrics

## jstack
- Stack Trace Tool
- Thread Analysis
- Deadlock Detection
- Thread Dump Output

## jmap
- Memory Analysis Tool
- Heap Dump Generation
- Memory Statistics
- Object Count

## jcmd
- Diagnostic Command Tool
- VM Operations
- Multiple Functions
- Production Friendly

## jstat
- Statistics Tool
- GC Statistics
- Memory Usage
- Compilation Statistics

## JVM Tuning
- Heap Size Configuration
- GC Algorithm Selection
- Compiler Optimization
- Throughput vs Latency

## Performance Optimization
- Profiling
- Bottleneck Identification
- Code Optimization
- GC Tuning
- Memory Management
