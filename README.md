# GIT Cheatsheet

Git makes use of SHA1 for hashing.
You can try hashing by using the command `git hash-object`

The `hash-object` command works with files and directories so you can't simply hash a string like this:

```bash
git hash-object "Apple Pie"
```

the above would throw an error.

To hash from the command-line, you can do something like this:

```bash
echo "Apple Pie" | git hash-object --stdin
```

This should return

```
23991897e13e47ed0adb91a0082c31c82fe0cbe5
```
