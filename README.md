# Cmdliner suburi

[dbuenzli/cmdliner: Declarative definition of command line interfaces for OCaml](https://github.com/dbuenzli/cmdliner)

## How to initialize project with cmdliner

```bash
dune init proj <project_name> --libs cmdliner
```

## How to add cmdliner to existing project

Add cmdliner to `lib/dune`.

```lisp
(library
 (name ocaml_cmdliner)
 (libraries cmdliner))
```

Add cmdliner to `bin/dune`.

```lisp
(executable
 (public_name ocaml_cmdliner)
 (name main)
 (libraries ocaml_cmdliner cmdliner))
```

## Development

```bash
dune exec ocaml_cmdliner
```

```bash
dune test
```

## Troubleshootings

### `Unbound module Cmd`

> Sorry these docs are for the (soon to be released) next version of cmdliner.
> For the current version use the docs from `odig doc cmdliner`.

https://github.com/dbuenzli/cmdliner/issues/133
