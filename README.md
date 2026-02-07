# Doxygen for Zed

A [Zed](https://zed.dev) extension for Doxygen documentation comment highlighting in C, C++, and other languages.

## Features

- Highlights Doxygen tags (`@brief`, `@param`, `@return`, `@see`, etc.)
- Parameter directions (`in`, `out`, `inout`)
- Code blocks (`@code` / `@endcode`)
- Identifier highlighting for parameter names
- Works inside `/** */`, `/*! */`, `///`, and `//!` comments

## Grammar

Uses a [WASM-compatible fork](https://github.com/ozacod/tree-sitter-doxygen) of [tree-sitter-doxygen](https://github.com/tree-sitter-grammars/tree-sitter-doxygen). The upstream grammar's external scanner uses C stdlib functions (`fprintf`, `isalnum`, `iswspace`) unavailable in Zed's WASM sandbox, so the fork replaces them with inline implementations.

## License

MIT
