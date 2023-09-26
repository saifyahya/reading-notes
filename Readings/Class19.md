## Puerly Functional Programming

- In purely functional programming, the state of a data structure is not changed directly. Instead, functional programming encourages the creation of new data structures with modified values, leaving the original data structures unchanged. This immutability ensures that functions do not have side effects and that changes to data are explicit and predictable.

- Purely functional programming is a programming paradigm that treats all computation as the evaluation of mathematical functions. It emphasizes immutability, referential transparency, and the absence of side effects. In purely functional programming, functions only depend on their input arguments and do not have access to or modify global or local state. It aims to ensure that the same input will always produce the same output, promoting predictability and ease of reasoning about code.

- Purely functional programming differs from many conventional programming approaches in several ways:

1. Immutability: In purely functional programming, data structures are typically immutable, meaning they cannot be modified once created. This contrasts with mutable data structures commonly used in imperative programming.

2. Referential Transparency: Purely functional programs strive for referential transparency, which means that a function's output is solely determined by its input, without any hidden state or side effects.

3. Avoidance of Side Effects: Purely functional programs minimize or eliminate side effects, such as modifying global variables or performing I/O operations within functions.

4. Emphasis on Functions: Functional programming relies heavily on functions as first-class citizens, enabling the composition of functions to build complex behavior.

5. Parallelism and Concurrency: Purely functional programs can be more amenable to parallel and concurrent execution due to their immutability and lack of shared state.

6. Persistent Data Structures: Purely functional programming often uses persistent data structures, which enable the creation of new versions of data structures without modifying the original ones.

In contrast, programs in imperative or object-oriented languages often involve mutable state, side effects, and a focus on the sequence of actions to achieve a desired outcome. Purely functional programming encourages a different mindset, where the emphasis is on expressing computations in a declarative and immutable manner.