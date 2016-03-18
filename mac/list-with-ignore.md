# List with ignore

If you want to filter out some files and folders to make a e.g. `git mv` operation on the rest you can issue the following command:

```bash
$ find . -maxdepth 1 ! -path "./.git" ! -path "./backend" ! -path "." ! -path "./frontend" | xargs -I '{}' git mv {} frontend
```

This command will filter out specific files provided with the -path parameter, then pipe the results and executes a further git mv on them.

Do not forget to exclude the . and .git paths as well.