# Prefixing lines from file

If you want to add extra prefix to input data obtained from a file per lines, you can use the following 'sed' command:
```bash
sed -e 's/^/http:\/\/my-domain.com\//' files-to-grab.txt
```

After prefixing the data and without overwriting the original input file's content, you may pipe the results in memory and execute a further commands, like 'wget', on them:

```bash
sed -e 's/^/http:\/\/my-domain.com\//' files-to-grab.txt | xargs wget -N --directory-prefix=/SAVED_LINKS
```

Notice, that -N enforces 'wget' here to update the already downloaded files without having them re-created and suffxied with new file names each time you execute the full command.



