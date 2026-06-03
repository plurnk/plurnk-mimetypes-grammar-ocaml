# @plurnk/plurnk-mimetypes-grammar-ocaml

Pre-built `tree-sitter-ocaml` WASM grammar for the [@plurnk/plurnk-mimetypes](https://github.com/plurnk/plurnk-mimetypes) framework.

## install

```
npm i @plurnk/plurnk-mimetypes-grammar-ocaml
```

## what's in here

- **`ocaml.wasm`** — pre-built from the pinned upstream [tree-sitter-ocaml](https://github.com/tree-sitter/tree-sitter-ocaml) commit (`grammars/ocaml` subdirectory) (SHA in `.grammar-pin`)
- `scripts/build-wasm.mjs` — reproducible rebuild from the pinned source
- `scripts/verify-wasm.mjs` — CI byte-identical reproducibility check

Declares only `web-tree-sitter` as a peer — no native `tree-sitter`, no node-gyp.

## license

MIT. The bundled `ocaml.wasm` is built from the upstream tree-sitter-ocaml grammar; see the pinned commit for that project's attribution.
