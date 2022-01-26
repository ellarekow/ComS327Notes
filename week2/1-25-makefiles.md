# make files

target- thing you are trying to build



```
target: dependency list
gcc file.x -Wall -Werror -o name
```


hello world program example: 

*makefile.txt*
```
hello:hello.c
    gcc hello.c -Wall -Werror -o hello
```

Then run command ```$ make```


### all of this is a rule!

to do all: 

```
all: file1 file2 file3

file1:file1.c
    gcc file1.c -Wall -Werror -o file1

file2:file2.c
    gcc file2.c -Wall -Werror -o file2 

file3:file3.c
    gcc file3.c -Wall -Werror -o file3
```

then run ```$ male``` as per usual

## Removing things in the make file: 

```
    clean: 
        rm -f *~ classfile.class outputfile core
```
dont usally need the classfile.class as it is for java

## partial compile
```
hello:hello.o
    gcc hello.o -o hello

hello.o:hello.c
    gcc -c hello.c -Wall -Werror
```

## Change log
name it CHANGELOG - simply a timestamp and what you did (aka commit messages)
```
// ex
Jan 19: started by creating a test
Jan 20: asdhfahs
Jan 21: ashdkfas
```

```git log``` will gnerate this file

# HOW TO SUBMIT
  *note this is in the syll*
  ## Connecting to the pyrite
  * ``` ssh netid@pyrite.cs.iastate.edu
    ```
  * ```git clone``` repo
  * compile and run repo
  * ```git log > CHANGELOG``` will gnerate this file

  ## creating the tar file (in terminal)
  * ```$ make clean```
  * go to parent directory
  * ```$ gentar```