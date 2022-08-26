add nnF to folder in a directory
```
 for dir in */ ; do mv "${dir}" "nnF ${dir}" ;done
```


rename all js to jsx
https://gist.github.com/mustafaturan/32df16bb4c49fbd837f777000f4b9aa2
```
for x in *.js; do mv "$x" "${x%.js}.jsx"; done
```
