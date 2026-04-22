# lmu-cmsi-3802-homework1

<p align="center">
  <img src="docs/RímereLogo.png" width="220">
</p>

<h1 align="center">Rímere</h1>

<h2 align="center">
  Computing for the Medieval World!
</h2>

---

## Overview

In an age before silicon-based screens, computation was the craft of scribes, scholars, and quiet thinkers. These were the people who transformed symbols into meaning. **Rímere** reimagines programming as it might have existed in that world: a language shaped not by modern syntax, but by the cadence and vocabulary of Old English.

Rather than calling functions or executing commands, a programmer in Rímere chants instructions, binds values, and declares truths using words inspired by a time when knowledge was handwritten and computation was an art. By blending historical language with modern programming principles, Rímere invites its users to experience coding as both logic and storytelling.

Rímere is not intended to be a perfectly reconstructed linguistic model of Old English. Instead, it is a **thematic programming language** that draws from Old English vocabulary and style while remaining readable, teachable, and implementable in a modern compiler project.

---

## Design Goals

- Create a programming language with a distinctive medieval identity
- Make syntax feel literary and narrative rather than purely mechanical
- Preserve core programming concepts in a form that is still understandable to modern users
- Balance novelty with usability so the language is fun to write and feasible to implement
- Explore how theme and syntax can shape the programmer’s experience

---

## Features

### Old English-inspired syntax

Rímere uses keywords and commands inspired by Old English vocabulary. For example, terms such as **bindan** (“to bind”), **sprecan** (“to speak”), **cweðan** (“to say, declare”), and **tellan** (“to count, reckon”) provide a fitting basis for assignment, output, declaration, and arithmetic-oriented operations.

### Readable, narrative-style code

Programs are written more like proclamations or instructions than dense symbolic expressions. The goal is for Rímere code to feel as though a scribe is recording commands, not merely typing machine directives.

### Strong thematic identity

Rímere is built around a consistent medieval world concept. Naming, syntax, examples, and semantics all reinforce the idea that programming is an act of inscription, declaration, and ordering.

### Familiar core programming constructs

Despite its stylized presentation, Rímere still supports recognizable programming ideas such as:

- variable binding
- expressions and evaluation
- conditionals
- repetition
- functions or named procedures
- boolean truth values
- numeric and textual data

This allows users to learn and use the language without sacrificing essential computational power.

### Minimal punctuation philosophy

Where possible, Rímere favors words and structure over symbol-heavy syntax. This helps the language feel older, more ceremonial, and more readable to humans.

### Beginner-friendly semantics

Even though the syntax is themed, the semantics are meant to stay approachable. A user should be able to infer what the code is doing from the wording and structure of the statements.

### Expressive naming conventions

Identifiers in Rímere can follow the aesthetic of chronicles, titles, or invocations, encouraging code that feels authored rather than assembled.

### Clear separation between declaration and action

One of the core stylistic goals of Rímere is distinguishing between:

- declaring what is true
- binding what is known
- commanding what should happen

That distinction gives the language a more deliberate and ceremonial feel.

---

## Checks

Rímere is designed with compile-time and runtime discipline in mind. Its checks aim to make programs easier to reason about while preserving the language’s expressive style.

### Static

The following checks should be performed before execution:

- **Undefined name detection**  
  Variables, functions, or symbols must be declared before they are used.

- **Duplicate declaration prevention**  
  The same identifier should not be declared multiple times in the same scope unless shadowing is explicitly allowed.

- **Type-consistency checks**  
  Expressions should be validated so that incompatible values are not combined incorrectly.

- **Arity checking**  
  Invocations of procedures or functions must supply the correct number of arguments.

- **Scope validation**  
  Names should only be accessible within valid regions of the program.

- **Syntactic structure enforcement**  
  Statements must follow the grammar of the language and preserve the intended narrative structure.

### Safety

Rímere should aim to protect programmers from common errors through language design:

- **Explicit declarations**  
  Values should be introduced intentionally rather than appearing implicitly.

- **Controlled mutation**  
  Rebinding or reassignment should be visible and deliberate.

- **Predictable evaluation**  
  Expressions should execute in a clear and consistent order.

- **Readable failure messages**  
  Errors should explain what went wrong in language that matches the style of the project without becoming cryptic or overly theatrical.

- **Optional immutability support**  
  Certain bindings may be treated as fixed truths once declared.

### Security

Although Rímere is an academic language and not a production system, its design should still consider safe execution practices:

- **No arbitrary code execution from string input**
- **Restricted runtime environment**
- **Validated parsing of all source text**
- **No implicit access to files, system resources, or external processes unless explicitly provided**
- **Clear boundaries between language features and host-language implementation**

These measures help ensure that the language remains controlled, predictable, and appropriate for classroom use.

---

## Example/Comparison Programs

Below is a conceptual comparison between modern programming style and the style Rímere aims to capture.

### Variable Assignment

#### Python Vs Rimere

```python
x = 5
```
```rimere
bindan x as 5
```
```python
print("Hello, world!")
```
```rimere
sprecan "Wes þu hal!"
```
```python
if x > 10:
    print("greater")
else:
    print("lesser or equal")
```
```rimere
gif x > 10
    sprecan "maerra"
elles
    sprecan "laessan oððe gelic"
```

