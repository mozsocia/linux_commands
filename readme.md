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

### delete folder recursively

```
find . -type d -name "foo" -exec rm -rf {} +
```

```
find . -type d -name "bar" -exec rm -rf "{}" \;


find . -type d -name "foo" -exec rm -rf {} + -print
```

https://linuxhint.com/linux-find-command-tutorial/

https://askubuntu.com/questions/339015/what-does-mean-in-the-find-command


### rar file make into parts

https://superuser.com/questions/396813/how-do-i-rar-a-file-into-several-parts-in-linux

```
sudo apt-get install rar

rar a -v50m first.rar folder_name
```



### Copy Using Linux
 path that contains folder you want to copy
 ```
%cd /gdrive/My Drive/...
%cp -av YOUR_FOLDER NEW_FOLDER_COPY
```
If you’re wondering what % is for, it’s simply the Google Colab way of signaling to the notebook to run a Linux terminal command.


### size of a directory
https://linuxize.com/post/how-get-size-of-file-directory-linux/

```
du -sh dir_name
```



https://askubuntu.com/questions/633945/how-can-i-merge-multiple-directories-into-one
