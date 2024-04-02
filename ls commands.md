To show only directories with the `ls` command in Bash, you can use the following options:

1. `ls -d */`
   - This command lists only directories in the current working directory.
   - The `*/` pattern matches all directories, and the `-d` option prevents `ls` from listing the contents of those directories.

2. `ls -ld */` or `ls -l */`
   - These commands provide a long listing format (`-l`) for directories only.
   - The `-d` option prevents `ls` from listing the contents of those directories, while the `*/` pattern matches all directories.

3. `ls -d *[/]` (with square brackets)
   - This command also lists only directories in the current working directory.
   - The `*[/]` pattern matches any entry that ends with a forward slash (`/`), which are directories in Unix-like systems.

4. `ls -l | grep '^d'`
   - This command lists all entries (including files and directories) in long format, and then pipes the output to the `grep` command.
   - The `grep '^d'` filters the output to show only lines starting with `d`, which represents directories in the long listing format.

You can combine these options with other `ls` options, such as `-a` to include hidden directories, `-h` for human-readable file sizes, or `--color=auto` for colorized output.

For example, `ls -ld *[/] -h --color=auto` will show a long listing of directories with human-readable sizes and colorized output.

Note that these commands will only list directories in the current working directory. If you want to list directories in a different location, you'll need to provide the path to that location before the command (e.g., `/path/to/directory ls -d */`).
