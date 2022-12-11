# Examples

<details><summary>List files in current directory</summary>

`ls` is the "list" command, which lists files in the working directory.

```bash
ls          # show me the files in my current directory
ls /tmp     # show me the files in the '/tmp' directory

echo $HOME  # show me the value of the `HOME` variable
ls $HOME    # show me the files in the $HOME directory

echo 'arg with spaces' 'second arg'
echo "\$HOME is interpolated to: $HOME"
```

</details>

<details><summary>Find a string within source files</summary>

```bash
find .         \
  -name '*.rs' \
  -type f      \
  -not -path './target/*' |
xargs grep '"Error\b'

# with ripgrep
rg -Fw '"Error'
```

</details>
