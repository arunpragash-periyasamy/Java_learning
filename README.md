# Java Learning

A personal collection of Java exercises, assignments, and LeetCode solutions written while
learning core Java and data structures & algorithms. Each topic lives in its own folder, most of
them set up as standalone IntelliJ IDEA projects.

## Status

Prototype / practice collection — this is a learning repo, not a packaged application. There's no
build tool (no Maven/Gradle), no test suite, and no CI. Files are run individually from an IDE or
with `javac`/`java`.

## What's covered

| Folder | Topic | Files |
|---|---|---|
| `intellij-programs/FirstProgram` | Java basics: primitives, input, sums, temperature conversion | 9 |
| `intellij-programs/ConditionalsAndLoops` | If/else, loops, Fibonacci, digit counting, number reversal | 8 |
| `intellij-programs/Functions` | Methods: overloading, varargs, scope, shadowing, recurs/string helpers | 12 |
| `intellij-programs/ArraysAndArrayList` | Arrays vs ArrayList, multi-dimensional arrays, reversing, swapping | 9 |
| `intellij-programs/LinearSearch` | Linear search over arrays, 2D arrays, ranges, strings | 6 |
| `intellij-programs/Binary Search` | Binary search, order-agnostic binary search | 2 |
| `intellij-programs/BitwiseOperator` | Bit manipulation: parity, set bits, power of two, XOR range | 10 |
| `intellij-programs/Sorting` | Bubble/insertion/selection sort, cyclic sort, array rotation | 13 |
| `intellij-programs/Recursion` | Large recursion set: factorial, permutations, subsets, merge/quick sort, sliding window, patterns | 44 |
| `intellij-programs/Recursions` | Smaller recursion set (Fibonacci, binary search, messages) | 6 |
| `intellij-programs/BackTracking` | Maze-solving problems (all paths, obstacles, diagonals) | 7 |
| `intellij-programs/Maths` | GCD, primes, sieve, Newton's sqrt, factors | 7 |
| `intellij-programs/PrintingPatterns` | Console pattern printing | 2 |
| `intellij-programs/Strings` | String comparison, palindromes, string methods | 6 |
| `intellij-programs/Switch` | Switch statement example | 1 |
| `dataStructures/LinkedList` | Singly/doubly linked list implementations from scratch | 4 |
| `java_assignments/first_java` | Early assignments: Armstrong numbers, currency conversion, palindromes | 9 |
| `java_assignments/FlowOfProgram` | HCF/LCM, leap year, multiplication table | 5 |
| `java_assignments/ConditionalAndLoops` | Area/interest/discount calculations, factorials, factors | 13 |
| `java_assignments/FunctionOrMethods` | Largest/smallest of three, basic methods | 2 |
| `java_assignments/BinarySearch` | Binary search variants: ceiling/floor, rotated array, matrix search | 8 |
| `java_assignments/Switch` | Switch statement example | 1 |
| `java_practice_questions` | Loose array practice problems (no IDE project wrapper) | 5 |
| `LeetcodeSolutions/Arrays` | LeetCode array problems (candies, matrix diagonal sum, good pairs, etc.) | 7 |
| `LeetcodeSolutions/String` | LeetCode string problems (defanging IPs, string halves, IP parsing, etc.) | 8 |
| `OOPS/exceptionHandling` | Try/catch exception handling basics | 3 |

207 `.java` files in total across the repo.

## Tech stack

- **Java** (JDK) — no framework or library dependencies.
- Most subfolders are standalone **IntelliJ IDEA** projects (`.iml` file + `.idea/` config).
- `.idx/dev.nix` configures a [Project IDX](https://idx.google.com) / Firebase Studio workspace
  with an OpenJDK JRE, for running the repo in a cloud dev environment.

## Folder structure

```
dataStructures/        # Data structure implementations (linked lists)
intellij-programs/     # Topic-by-topic IntelliJ projects: basics, loops, arrays, search,
                        # sorting, recursion, backtracking, math, strings, patterns
java_assignments/       # Coursework-style assignments, grouped by topic
java_practice_questions/ # Standalone array practice files (no IDE project wrapper)
LeetcodeSolutions/      # LeetCode problems grouped by category (Arrays, String)
OOPS/                   # Object-oriented programming exercises (exception handling)
```

## Getting started

Each topic folder with a `src/` directory and `.iml` file is a self-contained IntelliJ IDEA
project — open the folder in IntelliJ and run any file containing a `main` method.

To run a file directly from the command line instead:

```bash
javac path/to/File.java
java -cp path/to ClassName
```

Some files declare a package (e.g. `dataStructures.LinkedList`) and must be compiled/run from the
repository root with the matching package path, e.g.:

```bash
javac dataStructures/LinkedList/*.java
java -cp . dataStructures.LinkedList.Main
```
