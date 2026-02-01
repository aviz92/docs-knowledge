# Design Patterns Reference
Comprehensive list of design patterns organized by category.

---

## Creational Patterns
Patterns that deal with object creation mechanisms.

### 1. Abstract Factory
Creates families of related objects without specifying their concrete classes.
**Use when:** You need to create families of related objects that must work together.

### 2. Builder
Constructs complex objects step by step, allowing different representations.
**Use when:** You need to create complex objects with many optional parameters.

### 3. Factory Method
Creates objects through a common interface, letting subclasses decide which class to instantiate.
**Use when:** You want to delegate object creation to subclasses.

### 4. Prototype
Creates new objects by copying existing ones (cloning).
**Use when:** Object creation is expensive, and you can clone existing instances.

### 5. Singleton
Ensures a class has only one instance and provides global access to it.
**Use when:** You need exactly one instance of a class (database connections, loggers).

### 6. Object Pool
Reuses expensive-to-create objects instead of creating new ones.
**Use when:** Object creation is costly, and you need many short-lived objects.

---

## Structural Patterns
Patterns that deal with object composition and relationships.

### 7. Adapter
Allows incompatible interfaces to work together by wrapping an object.
**Use when:** You need to use a class with an incompatible interface.

### 8. Bridge
Separates abstraction from implementation, allowing them to vary independently.
**Use when:** You want to avoid a permanent binding between abstraction and implementation.

### 9. Composite
Composes objects into tree structures to represent part-whole hierarchies.
**Use when:** You need to represent tree structures and treat individual objects and compositions uniformly.

### 10. Decorator
Adds behavior to objects dynamically without altering their structure.
**Use when:** You need to add responsibilities to objects at runtime.

### 11. Facade
Provides a simplified interface to a complex subsystem.
**Use when:** You want to provide a simple interface to a complex system.

### 12. Flyweight
Shares state to support many fine-grained objects efficiently.
**Use when:** You need to support large numbers of objects with minimal memory.

### 13. Proxy
Provides a placeholder or surrogate for another object to control access.
**Use when:** You need to control access to an object (lazy loading, access control, logging).

---

## Behavioral Patterns
Patterns that deal with communication between objects.

### 14. Chain of Responsibility
Passes requests along a chain of handlers until one handles it.
**Use when:** You want to give multiple objects a chance to handle a request.

### 15. Command
Encapsulates requests as objects, allowing parameterization and queuing.
**Use when:** You need to parameterize objects with operations, queue operations, or support undo.

### 16. Interpreter
Defines a grammar and interprets sentences in that language.
**Use when:** You need to interpret a language or expression.

### 17. Iterator
Provides a way to access elements of a collection sequentially without exposing its structure.
**Use when:** You need to traverse different data structures uniformly.

### 18. Observer
Notifies multiple objects about state changes in a subject.
**Use when:** Changes to one object require changing other objects, and you don't know how many.

### 19. State
Allows an object to alter its behavior when its internal state changes.
**Use when:** An object's behavior depends on its state, and it has many conditional statements.

### 20. Strategy
Defines a family of algorithms, encapsulates each, and makes them interchangeable.
**Use when:** You have multiple ways to perform a task and want to choose at runtime.

---

## Python-Specific Patterns
Patterns that leverage Python's unique features.

### 21. Context Manager
Manages resources with `with` statements for automatic cleanup.
**Use when:** You need guaranteed resource cleanup (files, database connections).

### 22. Descriptor
Customizes attribute access through `__get__`, `__set__`, `__delete__`.
**Use when:** You need fine-grained control over attribute access.

### 23. Metaclass
Customizes class creation and behavior.
**Use when:** You need to modify class creation behavior (ORM, validation).

### 24. Decorator Pattern (Function Decorators)
Python's `@decorator` syntax for wrapping functions.
**Use when:** You need to add behavior to functions without modifying them.

### 25. Generator Pattern
Lazy evaluation with `yield` for memory-efficient iteration.
**Use when:** You need to process large datasets without loading everything into memory.

---

## Architectural Patterns
High-level patterns for organizing application structure.

### 26. Repository Pattern
Abstracts data access logic, providing a collection-like interface.
**Use when:** You want to decouple business logic from data access.

### 27. Service Layer
Encapsulates business logic and coordinates between layers.
**Use when:** You need to organize business logic separately from presentation and data access.

### 28. Dependency Injection
Injects dependencies rather than hard-coding them.
**Use when:** You want loose coupling and testability.

### 29. Event-Driven Architecture
Components communicate via events rather than direct calls.
**Use when:** You need loose coupling and asynchronous communication.

---

## Concurrency Patterns
Patterns for managing concurrent execution.

### 30. Producer-Consumer
Coordinates data production and consumption between threads/processes.
**Use when:** You have separate producers and consumers working at different rates.

### 31. Active Object
Encapsulates method execution in its own thread.
**Use when:** You need asynchronous method execution.

### 32. Thread Pool
Reuses threads for multiple tasks instead of creating new ones.
**Use when:** You have many short-lived tasks to execute.

### 33. Lock
Synchronizes access to shared resources.
**Use when:** Multiple threads need to access shared data safely.

### 34. Future/Promise
Represents a value that will be available later.
**Use when:** You need to handle asynchronous operations and their results.

---

## Testing Patterns
Patterns for writing and organizing tests.

### 35. Test Fixture
Sets up and tears down test environment and data.
**Use when:** You need consistent test setup and cleanup.

### 36. Mock Object
Simulates behavior of real objects for testing.
**Use when:** You need to isolate units under test from dependencies.

### 37. Test Double
Generic term for mocks, stubs, fakes, and spies.
**Use when:** You need to replace real dependencies in tests.

---

## Integration Patterns
Patterns for integrating systems and services.

### 38. API Gateway
Single entry point for multiple services.
**Use when:** You have multiple microservices and need unified access.

### 39. Circuit Breaker
Prevents cascading failures by stopping requests when a service is down.
**Use when:** You need to handle service failures gracefully.

### 40. Retry
Automatically retries failed operations with backoff.
**Use when:** You need to handle transient failures.

### 41. Bulkhead
Isolates resources to prevent total failure.
**Use when:** You need to prevent one component's failure from affecting others.

---


## Resources

- [Design Patterns: Elements of Reusable Object-Oriented Software (Gang of Four)](https://en.wikipedia.org/wiki/Design_Patterns)
- [Refactoring Guru - Design Patterns](https://refactoring.guru/design-patterns)
- [Python Design Patterns](https://python-patterns.guide/)

