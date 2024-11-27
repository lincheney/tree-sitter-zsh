# tree-sitter-bash

## TODO
* [x] ANONYMOUS FUNCTIONS
* [x] PARAMETER EXPANSION
* [x] Parameter Expansion Flags
* [ ] ```Any character, or the matching pairs `(...)', `{...}', `[...]', or `<...>', may be used in place of a colon as delimiters```
* [ ] `case word in [ [(] pattern [ | pattern ] ... ) list (;;|;&|;|) ] ... esac`
* [ ] `repeat word do list done`
* [ ] `{ try-list } always { always-list }`
* [ ] `function [ -T ] word ... [ () ] [ term ] { list }`
* [ ] ALTERNATE FORMS FOR COMPLEX COMMANDS
* [ ] `>| word`, `>! word`, `>>| word`, `>>! word` `>&| word`, `>&! word`, `&>| word`, `&>! word`, `>>&| word`, `>>&! word`, `&>>| word`, `&>>! word`,
* [ ] `^^` logical XOR, `^^=`
* [ ] `=(...)`
* [ ] `${var[1][2]}`, `${var[2,4][2]}`
* [ ] Glob Operators
* [ ] Subscript Flags
* [ ] `$path[2]`
* [ ] `{ ... }` does not require semicolon
* [ ] `"${__stderr//'/'\''}"`
* [ ] `${${words[@]:-1}[(r)-p]}`
* [ ] mathematical functions `(( int(height / 3) ))`


---

[![CI][ci]](https://github.com/tree-sitter/tree-sitter-bash/actions/workflows/ci.yml)
[![discord][discord]](https://discord.gg/w7nTvsVJhm)
[![matrix][matrix]](https://matrix.to/#/#tree-sitter-chat:matrix.org)
[![crates][crates]](https://crates.io/crates/tree-sitter-bash)
[![npm][npm]](https://www.npmjs.com/package/tree-sitter-bash)
[![pypi][pypi]](https://pypi.org/project/tree-sitter-bash)

Bash grammar for [tree-sitter](https://github.com/tree-sitter/tree-sitter).

## Development

Install the dependencies:

```sh
npm install
```

Build and run the tests:

```sh
npm run build
npm run test
```

Run the build and tests in watch mode:

```sh
npm run test:watch
```

### References

- [Bash man page](http://man7.org/linux/man-pages/man1/bash.1.html#SHELL_GRAMMAR)
- [Shell command language specification](http://pubs.opengroup.org/onlinepubs/9699919799/utilities/V3_chap02.html)
- [mvdnan/sh - a shell parser in go](https://github.com/mvdan/sh)

[ci]: https://img.shields.io/github/actions/workflow/status/tree-sitter/tree-sitter-bash/ci.yml?logo=github&label=CI
[discord]: https://img.shields.io/discord/1063097320771698699?logo=discord&label=discord
[matrix]: https://img.shields.io/matrix/tree-sitter-chat%3Amatrix.org?logo=matrix&label=matrix
[npm]: https://img.shields.io/npm/v/tree-sitter-bash?logo=npm
[crates]: https://img.shields.io/crates/v/tree-sitter-bash?logo=rust
[pypi]: https://img.shields.io/pypi/v/tree-sitter-bash?logo=pypi&logoColor=ffd242
