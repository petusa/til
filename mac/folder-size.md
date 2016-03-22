# Folder size

If you want to obtain the size of a folder or files you can use the `du` command:

```bash
$ du -sh <FOLDER1_OR_FILE>
```

To e.g. comapre multiple folders' sizes at a time use the following:

```bash
$ du -sc <FOLDER1> <FOLDER2>
```

Result:
```bash
14924	<FOLDER1>
14924	<FOLDER2>
29848	total
```

Source: http://unix.stackexchange.com/questions/185764/how-do-i-get-the-size-of-a-directory-on-the-command-line
