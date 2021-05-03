# TypeScript Style guide

This also encompasses our JavaScript style. Please also ensure that you remain familiar with this document as it may change from time to time.

## Introduction

Good judgement should be followed. There may be times where it is more readable to not follow a particular guideline.
Readable code is preferred over code that strictly follows this guide.

Where useful, a short summary explaining why the guideline is in place is included to help explain the rationale behind having it.

Please note that we're using Yarn as our package manager, not npm.

## Files

### Include copyright notice

All source files should start with our [copyright notice](https://github.com/Project-Books/book-project/blob/react-login-558/COPYRIGHT) attached verbatim.

## Formatting

Lines should generally not exceed our 100 characters column limit. This is to be consistent with our Java style guide.

### Braces

#### One true brace style (1TBS)

We use the [One true brace style (1TBS)](https://en.wikipedia.org/wiki/Indentation_style#Variant:_1TBS_(OTBS)).

```ts
// bad: braces should be used even where it is optional to do so in if, else if, while and do statements
if (condition)
    doSomething();

// good
if (condition) {
    doSomething();
} else {
    doSomethingElse();
}
```

## Language

- Avoid using `var`. Instead, prefer `const` and `let`
- No wildcard imports (so we have one export per file)

## Naming

### Method names

Method names should be written in `camelCase` and be be verb or verb phrases.

### Enum names

Enum names should be written in `PascalCase`. Enum items are written in `CONSTANT_CASE`.

### Parameter names

Parameter names should be written in `camelCase`.

### Local variable names

Local variable names should be written in `camelCase` even where they are constants.

## Acknowledgements

Adapted from [Google's JavaScript style guide](https://google.github.io/styleguide/jsguide.html) and [Airbnb's JavaScript style guide](https://github.com/airbnb/javascript/blob/master/README.md).

