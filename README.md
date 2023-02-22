# ALX Simple shell project

# General Requirements

* Allowed editors: vi, vim, emacs
* All your files will be compiled on Ubuntu 20.04 LTS using gcc,
  using the options -Wall -Werror -Wextra -pedantic -std=gnu89
* All your files should end with a new line
* A README.md file, at the root of the folder of the project is mandatory
* Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
* Your shell should not have any memory leaks
* No more than 5 functions per file
* All your header files should be include guarded
* Use system calls only when you need to
* Write a README with the description of your project

**Output**

* Unless specified otherwise, your program must have the exact same output
  as sh (/bin/sh) as well as the exact same error output.
* The only difference is when you print an error, the name of the
  program must be equivalent to your argv[0]

**List of Allowed functions and System calls**

* access
* chdir
* close
* closedir
* execve
* exit
* \_exit
* fflush
* fork
* free
* getcwd
* getline
* gitpid
* isatty
* kill
* malloc
* open
* opendir
* perror
* read
* readdir
* signal
* stat
* lstat
* fstat
* strtok
* wait
* waitpid
* wait3
* wait4
* write

**Compilation**

`gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh`

# Testing

Your shell shouuld work like this in interactive mode:
```
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
```

But also in non-interactive mode:
```
$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
```

### Authors
**Dennis Augustine Kafui Kofi Adaku**
* `GitHub`: > @KafuiAdaku

**Timoty Obeng Nkrumah**
* `GitHub`: > @Papa-Obeng
