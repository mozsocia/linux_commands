### How to Remove Files and Directories Using Linux Command Line

https://linuxize.com/post/how-to-remove-files-and-directories-using-linux-command-line/



You can also use a wildcard (*) and regular expansions to match multiple files. For example, to remove all .pdf files in the current directory, use the following command:

```
rm *.pdf
```

### delete-matching-files-in-all-subdirectories

https://superuser.com/questions/112078/delete-matching-files-in-all-subdirectories

```
find . -name '*.pdf' -delete
```

TO that directory

```
find "/home/mozdalif/dir1/dir11/" -name '*.vtt' -delete
```




### rar file make into parts

https://superuser.com/questions/396813/how-do-i-rar-a-file-into-several-parts-in-linux

```
sudo apt-get install rar

rar a -v50m first.rar folder_name
```
