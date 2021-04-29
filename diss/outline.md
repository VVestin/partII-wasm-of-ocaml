# Compiling OCaml to WebAssembly
## Introduction
(notes):
- Clearly explain the problem
   - Why is the problem interesting
   - What does the solution enable?
- Describe what I've built
   - Explain how it solves the problem
   - Leave details for the implementation

- JavaScript is weird (dynamic types, unusual prototype-based inheritance, event loop paradigm)
- The web is an important platform for enterprise projects and would benefit from paradigms and techniques besides JS
- OCaml is well suited to software engineering, strong and provably sound type system
- WebAssembly has exciting performance and safety properties that JS lacks, can totally be a target for an OCaml compiler
- Running OCaml on the Web would enable cool things including better performance
- Description of what I've built and how it aims to solve the problem

## Preparation
(notes):
- Explain background knowledge needed
   - Rule of thumb: explain things outside of 1B
   - Explain things needed to make sense of decisions later
- Requirements analysis
   - Techniques and tools that could be used
   - What did I decide to use
   - What factors lead to these techniques
- Engineering practices that were followed
   - What are standard practice: validation & source control
   - How does what I did compare to standard practice

### Background
- How does webassembly work
    - JIT compiling JS and the V8 Engine
    - Overview of what WebAssembly is
    - Stack Machine w/ heap and 2/4 basic types
    - Talk about the important features of wasm for reference in the implementation chapter
    - WebAssembly Binary Toolkit use
- Talk about decision to use JavaScript
   - Running in Node/browsers possibilities
- Talk about ocamllex and ocamlyacc and jison
- Alternatives to using the ocaml compiler (ocaml to js, vanilla js) for reference in evaluation chapter
### Requirements
- Description of OCaml subset
- Development of sample programs
- Setup tools for automated testing
- Benchmarking for evaluation
### Engineering
- Iterative Development (instead of waterfall)
- Test Driven Development
- Kanban organizational technique
- Source control/backup tools

## Implementation
(notes):
- Explain the project itself
    - Describe repository layout
    - Design and methodology
    - Explain it as if they're a new hire
- How did the methods from the preparation apply to the project
- What did I try that didn't work?
- What was achieved, what does it do
    - Explain the limitations (gosh, there's a lot)

## Evaluation
(notes):
- Explain evaluation methods
    - Quantitative and qualitative results
- Give the results
- Compare with the success criteria
- Interpret what the results teach us

## Conclusion
(notes):
- What have you learned
- What would you do differently if done again
- What advice would I have for others doing this project

- Discuss the success criteria
- What did I learn from this project
- What would I do differently if doing project again