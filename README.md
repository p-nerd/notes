# notes
List of languages and their libraries

## Linux

- `echo <something>`
  - `echo Hello`
  - `echo $0`
- `whoami`
- `history`
- `!<line from history list>`
  - `!2`
- `apt`
- `pwd`
- `ls`
  - `ls -1`
  - `ls -l`
  - `ls /etc/apt`
- `cd`
  - `cd /etc/apt`
  - `cd ..`
  - `cd ~`
- `mkdir <directory name>`
- `mv <old_path> <new_path>`
- `touch <filename 1> <filename 2>`
- `rm <filename 1> <filename 2>`
  - `rm file*`
  - `rm -r <directory name>` remove the directory
- `cat <filename>`
  - `cat file1.txt file2.txt > combined.txt` -> combine two file
- `more <filename>` -> to see long file easily
- `less <filename>` -> replacement for more with more feature
- `head -n <line count> <filename>` -> see some line from top
  - `head -n 5 /etc/adduser.conf`
- `tail -n <line count> <filename>` -> see some line from bottom
  - `tail -n 5 /etc/adduser.conf`
- `grep` -> searching text
  - `grep hello file1.txt` -> case sensitive search
  - `grep -i hello file1.txt` -> case-insensitive search
  - `grep root /etc/passwd`
  - `grep root file1.txt file2.txt` -> search in multiple files
  - `grep root -r /etc` -> search in directory
- `find` -> finding files and directory
  - `find /etc -type d` -> finding only directory
  - `find /etc -type f` -> finding only files
  - `find /etc -type f -name "f*"` -> finding files that start with f
  - `find /etc -type f -iname "f*"` -> finding files that start with f or F
  - `find / -type f -name "*.py" > list_of_python_files.txt`
- chaining commands
  - `mkdir text ; cd text ; ls`
  - `mkdir text && cd text && ls`
  - `mkdir text || echo "directory already exits"`
- environment variables
  - `printenv`
  - `printenv PATH`
  - `echo $PATH`
  - `export DB_USER=shihab`
- process
  - `ps` -> list all the processes
  - `sleep 3 &` -> sleep process for 3 seconds
  - `kill <process id>`
- managing users
  - `adduser <user name>`
  - `useradd -m <user name>`
  - `usermod -s /bin/bash shihab2` -> chaining the user default shell
  - `userdel <user name>`
  - `cat /etc/passwd`
  - `cat /etc/shadow`
- managing groups
  - `addgroup <group name>`
  - `groupadd <group name>`
  - `cat /etc/group`
  - `usermod -G <group name> <user name>`
  - `groups <user name>` -> listing all groups of the user
- file permissions
  - `chmod u+x <filename>` -> for user add execute permissions
  - `chmod u-x <filename>` -> for user remove execute permissions


## Docker

## Libraries
  - CSS/Component Libraries
    - [x] [TailwindCSS](https://github.com/tailwindlabs/tailwindcss): Rapidly build modern websites without ever leaving your HTML.
    - [x] [daisyUI](https://github.com/saadeghi/daisyui): Use Tailwind CSS but write fewer class names
  - JS/TS/Node/Deno/Bun Libraries
    - [x] [Day.js](https://github.com/iamkun/dayjs/): Fast 2kB alternative to Moment.js with the same modern API
    - [ ] [Kysely](https://github.com/kysely-org/kysely): The type-safe SQL query builder for TypeScript
