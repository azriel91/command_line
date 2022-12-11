# Rust Alternatives

The following show alternatives to standard tools.

These generally have coloured output, and perform faster.


| Tool      | Alternative  |
|:----------|:-------------|
| cat       | bat          |
| cd        | z (zoxide)   |
| diff      | delta        |
| find      | fd           |
| grep      | rg           |
| ls        | lsd          |
| sed       | sd           |
| top       | btm (bottom) |
| powerline | starship     |


## Nushell

Like Powershell, nushell doesn't just pass strings between commands, but objects.

```bash
ls | sort-by type
ls | sort-by type | where size > 10kb

echo [[name value]; ['a' 1] ['b' 2] ['c' 3]] | table

echo [[name value]; ['a' 1] ['b' 2] ['c' 3]] |
  update value {|it| $it.value + 10 } |
  table
```
