# Relic Programming Language Tutorial Plan

This tutorial is aimed at programmers who have experience with at least one
mainstream programming language but are not necessarily experts. The tutorial
progressively introduces concepts of the Relic programming language through the
development of a single project. 

The application is: a terminal file explorer.

## Chapter 0: **Introduction and Basics**
**Title**: "Hello, Relic!"
- **Objective**: Introduction to the language, setting up a project, and writing your first program.
- **Relevant Specs**: core, extra
- **Content**:
  - Explain `def` for defining values.
  - Use `import` to bring in the terminal module.
  - Introduce `proc` for functions.
  - Write a "Hello, World!" program using `(write-line "Hello, World!")`.

## Chapter 1: **Types and Procedures**
**Title**: "Building Logical Blocks"
- **Objective**: Understanding Relic's strong typing and function definitions.
- **Content**:
  - Simple types like `I64`, `String`.
  - Typed functions using `(proc [(x I64)] (+ x 10))`.
  - Introduce lists and basic operations `(list 1 2 3)` (see spec/data/list/index.org).
  - Modify the program to accept user input, perform a computation, and print the result.

## Chapter 2: **Control Flow and Logic**
**Title**: "Deciding the Path"
- **Objective**: Conditional constructs and pattern matching.
- **Content**:
  - Explain `if` and `cond`.
  - Use `match` for pattern matching. Example: processing a custom `Result` Enum.
  - Extend the terminal-based application to include a decision-making feature based on user input.

## Chapter 3: **Structures and Dynamic Values**
**Title**: "Keeping Things Together"
- **Objective**: Introduce `struct` and `dynamic`.
- **Content**:
  - Define a `struct` to manage related data.
  - Access and manipulate fields using `.`.
  - Use `dynamic` values for scoped mutability.
  - Create a simple game state structure to track user sessions.

## Chapter 4: **Loops and Recursion**
**Title**: "Repeat Until Success"
- **Objective**: Leverage `labels`, `go-to`, and recursion.
- **Content**:
  - Write loops with `labels` and `go-to`.
  - Demonstrate recursion for sum calculations/multipliers.
  - Use these to create a small interactive program, e.g., a guess-the-number game.

## Chapter 5: **Polymorphism and Traits**
**Title**: "Generics and Beyond"
- **Objective**: Dive into `all` and traits for polymorphic functions.
- **Content**:
  - Create a generic function `(all [A] proc [(x A)] x)`.
  - Explain the power of traits like `Num`.
  - Show examples of generic functions operating across multiple types.
  - Extend the current project (e.g., the game) to introduce customizable play behaviors.

## Chapter 6: **Advanced Topics and Cleanup**
**Title**: "Tying It All Together"
- **Objective**: Teach advanced concepts and refine the project.
- **Content**:
  - Explain `seal` and `unseal` for advanced type security.
  - Use `instance` for typeclass implementations dynamically.
  - Add features such as a leaderboard with different levels of access and persistence.
