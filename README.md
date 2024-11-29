# tree-sitter-bash

## TODO
* [x] ANONYMOUS FUNCTIONS
* [x] PARAMETER EXPANSION
* [x] Parameter Expansion Flags
* [x] ```Any character, or the matching pairs `(...)', `{...}', `[...]', or `<...>', may be used in place of a colon as delimiters```
* [x] `case word in [ [(] pattern [ | pattern ] ... ) list (;;|;&|;|) ] ... esac`
* [x] `repeat word do list done`
* [x] `{ try-list } always { always-list }`
* [x] `function [ -T ] word ... [ () ] [ term ] { list }`
* [x] `for a b c in ...`
* [ ] ALTERNATE FORMS FOR COMPLEX COMMANDS
    * [x] `if list { list } [ elif list { list } ] ... [ else { list } ]`
    * [ ] `if list sublist`
    * [ ] `for name ... ( word ... ) sublist`
    * [ ] `for name ... [ in word ... ] term sublist`
    * [ ] `for (( [expr1] ; [expr2] ; [expr3] )) sublist`
    * [x] `foreach name ... ( word ... ) list end`
    * [x] `while list { list }`
    * [x] `until list { list }`
    * [ ] `repeat word sublist`
    * [x] `case word { [ [(] pattern [ | pattern ] ... ) list (;;|;&|;|) ] ... }`
    * [ ] `select name [ in word ... term ] sublist`
    * [ ] `function word ... [ () ] [ term ] sublist`
* [x] `>| word`, `>! word`, `>>| word`, `>>! word` `>&| word`, `>&! word`, `&>| word`, `&>! word`, `>>&| word`, `>>&! word`, `&>>| word`, `&>>! word`,
* [x] `^^` logical XOR, `^^=`, `||=`, `&&=`
* [x] `=(...)`
* [x] `${var[1][2]}`
* [ ] `${var[2,4][2]}`
* [x] Glob Operators
* [ ] Subscript Flags
* [x] `$path[2]`
* [x] `{ ... }` does not require semicolon
* [x] `"${__stderr//'/'\''}"`
* [x] `${${words[@]:-1}[(r)-p]}`
* [x] mathematical functions `(( int(height / 3) ))`
* [ ] If the option BARE_GLOB_QUAL is set, then a trailing set of parentheses containing no `|` or `(` characters (or `~` if it  is  special)  is taken as a set of glob qualifiers.  A glob subexpression that would normally be taken as glob qualifiers, for example `(^x)`, can be forced to be treated as part of the glob pattern by doubling the parentheses, in this case producing `((^x))`.
* [ ] `job ... &|`, `job ... &!`


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
