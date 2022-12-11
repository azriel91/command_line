# Paths

All applications, shell or not, run in a "working directory".

```bash
# Print the current working directory
pwd

# Same, but with the `PWD` environment variable
echo $PWD
```

The `cd` command changes the working directory.

```bash
# Create a directory at '/tmp/abc/def' and switch to it
mkdir -p /tmp/abc/def
cd /tmp/abc/def
```

> **Tip:** You can `cd -` to move to the directory you were last in.


## Relative and Absolute Paths

Paths without a top level root are interpreted to be relative to the current working directory.

* **Linux / OS X:** Root is `/` or `~`.
* **Windows:** Root is usually a drive letter `c:\`.

```bash
cd /tmp
cd abc/def # relative to '/tmp'
```


## Special Paths


```bash
# '.' (dot) is a path referring to the current working directory
pwd
cd . && pwd


# '..' (dot dot) is a path referring to the parent of the current directory
cd .. && pwd


# '~' (tilde) is a notation for "current user's home directory"
cd ~ && pwd


# '/tmp' is usually a file system that lives on memory.
# It gets wiped when you restart your computer.
cd /tmp
```
