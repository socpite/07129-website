1. why did we move from punch cards to programming languages? what does that tell you about the purpose of programming languages?

we moved away from punch cards because they were cumbersome: hard to read, easy to damage, and slow to work with. they also forced programmers to work at a very low level, with none of the abstractions we now rely on. programming languages were developed to let humans express algorithms in a more natural and structured way. their purpose is not just to tell the computer what to do, but also to help humans think about, organize, and manage complexity in software. features like abstraction, modularity, and error checking make programming languages tools for both communication with machines and collaboration among humans.

2. there are hundreds of different programming languages out there. why do you think we need so many?

different languages are designed to solve different kinds of problems. for example, python emphasizes simplicity and readability, making it great for data analysis, scripting, and rapid prototyping. c provides low-level control and efficiency, which is essential for operating systems or embedded systems. some languages are built for safety (like rust), some for concurrency (like go), and others for domain-specific tasks (like sql for databases). having many languages means developers can choose the right tool for the job, rather than forcing one language to fit every scenario.

3. what are some drawbacks of a programming language you use? how would you like it to be different?

- python: while flexible, it can be too permissive. for example, accidentally overwriting a function name or relying on dynamic typing can introduce subtle bugs. python is also relatively slow due to limited compile-time optimization and its interpreted nature. many libraries address this by wrapping optimized c code, but i wish python had stronger built-in safeguards and more performance-focused features without sacrificing readability.

- rust: rust prioritizes safety and performance but at the cost of complexity. its steep learning curve, with concepts like ownership, borrowing, and lifetimes, can make code harder to read for newcomers. if rust could simplify some syntax or provide more gradual “onboarding” features, it would be more approachable while still retaining its strengths.

4. if you were going to create a new programming language, how would you start? what do you need to define?

the first step would be defining the purpose of the language: what kinds of problems it should solve and who the intended users are. for example, is it meant for scientists, system developers, or web programmers? once the goal is clear, i would gather input from potential users to identify the features they value most. after that, i would define the language’s fundamentals: its syntax, type system, data structures, and control flow. finally, i would build a minimal compiler or interpreter to test the design in practice, refining it based on feedback and real-world use cases.
