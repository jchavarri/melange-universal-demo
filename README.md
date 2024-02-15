# melange-universal

See [related discussion](https://github.com/melange-re/melange/discussions/694)
in the Melange repo.

A demo project template that showcases how to build a Melange library and an
OCaml library that share the same structure but with different implementation
using [Dune
contexts](https://dune.readthedocs.io/en/stable/overview.html#term-build-context).

The project currently uses a custom version of Dune from
[ocaml/dune#9839](https://github.com/ocaml/dune/pull/9839/).

## Quick Start

```shell
npm run init

dune build
```

## Differences with the Melange opam template

The main difference with the `melange-opam-template` is that all Melange
artifacts like generated `.js` files are placed in `_build/melange` rather than
in `_build/default`.

## Todo

- Editor integration seems to be broken for the Melange context
- Dune should show the context where a build error has happened on the terminal
  output (at least when it's not the `default` context)
