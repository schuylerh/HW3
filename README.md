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

# How to Guarantee Resource Safety in Software Development?

ChatGPT4's Response:
>1. Use Automatic Resource Management
>Garbage Collection
>Definition: An automatic memory management system that reclaims memory occupied by objects no longer in use.
>Reference Counting
>Definition: Keeps track of the number of references to a resource; when the count reaches zero, the resource is deallocated.
# References

# Relevant Concepts
