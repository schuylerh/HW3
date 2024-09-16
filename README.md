# LLM_Literature_Review


# IDENTIFICATION
- NAME: Schuyler Huang
- ASSIGNMENT: Influence of different programming paradigms (e.g., procedural, object-oriented, functional) on the development of modern programming languages
- LLM Used: ChatGPT-4
- DATE: September 15, 2024

# Assignment Description
This file documents my usage of an LLM to explore the topic of the influence of different programming paradigms on the development of modern programming languages.

# LLM Literature Review

## What are the key differences between these paradigms, and how do they affect language design choices?

ChatGPT4's Response:
>Procedural Languages prioritize linear execution and straightforward procedures, leading to languages that are simple and close to hardware but may require more effort to manage complex systems.
>
>Object-Oriented Languages focus on modeling real-world entities and their interactions, resulting in languages that support encapsulation, inheritance, and polymorphism to manage complexity in large software systems.
>
>Functional Languages emphasize immutability and pure functions, leading to languages that facilitate reasoning about code behavior, enable easier parallelization, and reduce side effects.
>

I liked ChatGPT's response here because of the comparisons that it is making for each paradigm. It relates procedural languages to hardware because they provide features and abstractions that map closely to the way computer hardware operates. Procedural langauges offer more control over the system's performance and behavior. For example, procedural langauges like C provide pointers that allow programmers to write and read specific memory locations directly. 

Object Oriented Languages is related to modeling real world entities. For example, a car would be represented by a car class and attributes such as the make and model. This helps to manage complexity and keep things organized. 

## What lessons from the evolution of programming paradigms can inform future language development?

ChatGPT4's Response:
>1. Embracing Multiparadigm Approaches
>Lesson Learned:
>
>No single paradigm is a one-size-fits-all solution. Languages like Python, Scala, and Rust successfully integrate multiple paradigms to provide flexibility.
>
>Implication for Future Languages:
>
>Flexibility: Designing languages that support procedural, object-oriented, functional, and other paradigms allows developers to choose the best approach for a given problem.
>Interoperability of Paradigms: Seamless integration between paradigms within a language enhances productivity.
>
>2. Concurrency and Parallelism as Core Features
>Lesson Learned:
>
>With the rise of multi-core processors, languages need to handle concurrency effectively.
>Models like Actor Model in Erlang and Akka, and async/await patterns address concurrency challenges.
>Implication for Future Languages:
>
>Concurrency Primitives: Provide built-in support for concurrency and parallelism, making it easier to write efficient, concurrent programs.
>Safe Concurrency Models: Emphasize models that reduce complexity, such as message passing over shared memory.
>
>3. Memory Safety and Resource Management
>Lesson Learned:
>
>Languages like C offer control but are prone to memory errors.
>Rust introduces a novel ownership model to ensure memory safety without a garbage collector.
>Implication for Future Languages:
>
>Automatic Memory Management: Incorporate garbage collection or safe manual memory management to prevent common errors.
>Resource Safety Guarantees: Language features that enforce safe handling of resources can reduce bugs.

ChatGPT pointed out several main lessons to keep track of when creating a new programming language. Firstly, programming languages that are inflexible are not known to be very successful, multiple paradigms integrated together to provide flexibility is a good feature to have. Secondly, multi-core processors are rising in usage and programming languages should be able to utilize all of these resources with concurrency. To be an effective and optimal programming language, parallelism and concurrency should be easy to write. Lastly, memory. The programming langauge should be able to manage memory safely without frequently running into errors.

## How to Guarantee Resource Safety in Software Development?

ChatGPT4's Response:
>1. Use Automatic Resource Management
>Garbage Collection
>Definition: An automatic memory management system that reclaims memory occupied by objects no longer in use.
>
>Reference Counting
>Definition: Keeps track of the number of references to a resource; when the count reaches zero, the resource is deallocated.
>
>2. Use Smart Pointers
>Definition: Objects that manage the lifetime of dynamically allocated memory through automatic deallocation.
>
>Prevents memory leaks by ensuring memory is freed when no longer needed.
>Reduces the risk of dangling pointers.
>
>3. Leverage RAII (Resource Acquisition Is Initialization)
>Definition: A programming idiom where resource allocation and deallocation are tied to object lifetime.
>
>Implementation:
>
>Resources are acquired in an object's constructor.
>Resources are released in the object's destructor or when it goes out of scope.
>
In order to create an optimal programming language in the future, ChatGPT said resource safety is required. I explored this topic and wanted to know about ways to implement it. ChatGPT provided several methods, and three of them were resource management, smart pointers, and leveraging RAII. 

## How to Ensure a Programming Language Supports Concurrency

ChatGPT4's Response:
># Key Strategies to Support Concurrency in a Programming Language
>
>## 1. Choose an Appropriate Concurrency Model
>-Thread-Based Concurrency: Uses threads within a process to execute tasks concurrently.
>-Event-Driven Concurrency: Employs an event loop to handle tasks asynchronously.
>-Actor Model: Encapsulates state and behavior within "actors" that communicate via message passing.
>-Communicating Sequential Processes (CSP): Processes interact through message passing over channels.
>-Software Transactional Memory (STM): Manages concurrent access to shared memory using transactions.>
>
>## 2. Provide Concurrency Primitives
>-Threads or Lightweight Processes:  Allow the creation and management of concurrent execution units.
>-Coroutines: Support functions that can pause and resume execution.
>-Asynchronous Functions: Enable non-blocking operations.
>
>## 3. Implement Synchronization Mechanisms
>-Locks and Mutexes: Control access to shared data to prevent race conditions.
>-Semaphores: Manage resource availability in concurrent environments.
>-Atomic Operations: Ensure certain operations complete without interruption.
>-Channels or Message Queues: Facilitate safe communication between concurrent entities.
>
Another factor that needs to be considered in creating a new programming language is concurrency. To support this, several requirements were provided by ChatGPT. An appropriate concurrency model is needed so that processes can be executed synchronously.

## What kind of type inference is trending and should be used in future programming languages?

ChatGPT4's Response:
># Current Trends in Type Inference:
>
>## 1. Local Type Inference
>
>Description: The compiler infers types within a local scope, such as the type of a variable based on its initializer.
>
>## 2. Global Type Inference with Hindley-Milner Algorithm
>
>Description: A classical type inference algorithm that infers types globally across the entire program.
>
>## 3. Bidirectional Type Inference
>
>Description: Combines both bottom-up and top-down inference, where the compiler uses context to infer types more effectively.
>
># Recommendations for Future Programming Languages
>## Support Local Type Inference with Option for Explicit Types
>
>Why: Provides flexibility for developers to omit types when they are obvious but specify them when clarity is needed.
>
>## Adopt Bidirectional Type Inference
>
>Why: Balances the need for explicitness and inference, handling complex types while keeping the inference process understandable.

# Notable Researchers
- Alan Kay: Pioneer of object-oriented programming.
- John McCarthy: Creator of Lisp and early contributor to functional programming.
- Barbara Liskov: Contributions to data abstraction and type systems.
- Martin Odersky: Creator of Scala, blending object-oriented and functional programming.
- Joe Armstrong: Co-creator of Erlang, emphasizing concurrency and fault tolerance.

# References
[Type Inference](https://repository.arizona.edu/bitstream/handle/10150/668754/azu_etd_hr_2023_0229_sip1_m.pdf?sequence=1&isAllowed=y).

[Memory Safety and Resource Management](https://www.proquest.com/docview/2447559736?pq-origsite=gscholar&fromopenview=true&sourcetype=Dissertations%20&%20Theses).

[Concurrency](https://scg.unibe.ch/archive/papers/Nier95bOOSC.pdf#page=49).
