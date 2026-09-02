# Rustlings

[![Rust](https://img.shields.io/badge/rust-1.97.1-CE422B?logo=rust&logoColor=white)](https://www.rust-lang.org)
[![Rustlings](https://img.shields.io/badge/rustlings-6.5.0-000000?logo=rust&logoColor=white)](https://github.com/rust-lang/rustlings)
[![Exercises](https://img.shields.io/badge/exercises-94-blue)](exercises/)
[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/rust-lang/rustlings/blob/main/LICENSE)

A personal working copy of [Rustlings](https://github.com/rust-lang/rustlings): 94 small exercises
covering the Rust language, from variables and control flow through ownership, traits, lifetimes,
and concurrency.

Each exercise is a source file that fails to compile, fails its tests, or trips a Clippy lint. The
task is to repair it. The watch mode rebuilds the current exercise on every save and prints the
compiler diagnostic alongside the exercise hint.

## Getting Started

```bash
rustlings            # interactive watch mode; the primary workflow
rustlings run        # run the current exercise once
rustlings hint       # print the hint for the current exercise
rustlings reset      # restore the current exercise to its original state
rustlings list       # show all exercises and their status
```

Watch mode key bindings: `n` next, `r` run, `h` hint, `l` list, `c` check all, `x` reset, `q` quit.

## Repository Layout

```
.
├── exercises/     # the exercises; all work happens here
├── solutions/     # reference solutions, to be consulted after an attempt
├── Cargo.toml     # one [[bin]] target per exercise
└── rust-analyzer.toml
```

Progress is recorded in `.rustlings-state.txt`, created on first run and excluded from version
control.

## Exercise Index

| No. | Section | Count | Topic | Book |
|-----|---------|:-----:|-------|------|
| 00 | `intro` | 2 | Introduction to the exercise format | — |
| 01 | `variables` | 6 | Bindings, mutability, shadowing | 3.1 |
| 02 | `functions` | 5 | Functions, parameters, return values | 3.3 |
| 03 | `if` | 3 | Conditionals as expressions | 3.5 |
| 04 | `primitive_types` | 6 | Scalars, tuples, slices | 3.2, 4.3 |
| 05 | `vecs` | 2 | `Vec<T>` and iteration | 8.1 |
| 06 | `move_semantics` | 5 | Ownership and borrowing | 4.1–4.2 |
| 07 | `structs` | 3 | Structs and methods | 5.1, 5.3 |
| 08 | `enums` | 3 | Enumerations and `match` | 6, 18.3 |
| 09 | `strings` | 4 | `String` versus `&str` | 8.2 |
| 10 | `modules` | 3 | Modules, `pub`, `use` | 7 |
| 11 | `hashmaps` | 3 | `HashMap<K, V>` | 8.3 |
| 12 | `options` | 3 | `Option<T>` and `if let` | 10.1 |
| 13 | `error_handling` | 6 | `Result`, `?`, custom error types | 9 |
| 14 | `generics` | 2 | Generic types | 10 |
| 15 | `traits` | 5 | Traits and implementations | 10.2 |
| 16 | `lifetimes` | 3 | Reference lifetimes | 10.3 |
| 17 | `tests` | 3 | `#[test]` and assertions | 11.1 |
| 18 | `iterators` | 5 | `Iterator`, `map`, `collect` | 13.2–13.4 |
| 19 | `smart_pointers` | 4 | `Box`, `Rc`, `RefCell`, `Cow` | 15, 16.3 |
| 20 | `threads` | 3 | Threads, `Arc`, channels | 16 |
| 21 | `macros` | 4 | `macro_rules!` | 20.5 |
| 22 | `clippy` | 3 | Lints and idiomatic code | — |
| 23 | `conversions` | 5 | `From`, `Into`, `TryFrom`, parsing | — |
| — | `quizzes` | 3 | Cumulative review exercises | — |

Chapter references point to [The Rust Programming Language](https://doc.rust-lang.org/book/).

## Working Through the Exercises

1. Run `rustlings`; it opens the first unfinished exercise.
2. Locate the `// TODO:` comment in the file and fix the code. Saving triggers a rebuild.
3. Read the compiler diagnostic in full; in Rust it frequently contains the fix verbatim.
4. Press `h` for the hint after roughly ten minutes without progress.
5. Consult `solutions/` only after a working attempt, to compare approaches.

## References

- [The Rust Programming Language](https://doc.rust-lang.org/book/) — the primary text
- [Rust by Example](https://doc.rust-lang.org/rust-by-example/) — the same material in code
- [Standard library documentation](https://doc.rust-lang.org/std/)
- [Clippy lint index](https://rust-lang.github.io/rust-clippy/master/) — rationale for each lint
