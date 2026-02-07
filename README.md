# Doxygen for Zed

A [Zed](https://zed.dev) extension that adds syntax highlighting for [Doxygen](https://www.doxygen.nl/) documentation comments in C, C++, and other languages.

## Features

- Syntax highlighting for Doxygen tags (`@brief`, `@param`, `@return`, `@see`, etc.)
- Parameter direction keywords (`in`, `out`, `inout`)
- Code block support (`@code` / `@endcode`)
- Identifier highlighting for referenced parameter names
- Works automatically inside `/** */`, `/*! */`, `///`, and `//!` comment blocks

## Installation

1. Open Zed
2. Open the Extensions panel (`zed: extensions` from the command palette)
3. Search for "Doxygen"
4. Click Install

## How It Works

Doxygen is registered as a hidden, injection-only language. Zed's built-in C and C++ language support already includes injection rules that activate Doxygen highlighting inside documentation comments. This extension provides the tree-sitter grammar and highlight queries that those injections target.

## Grammar

Uses [tree-sitter-doxygen](https://github.com/tree-sitter-grammars/tree-sitter-doxygen) for parsing.

## License

MIT
