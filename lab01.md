More information can be found here: https://wiki.ittc.ku.edu/ittc_wiki/index.php/EECS168:Lab1

## Objectives:
- Get familiar with Linux environment.
- Use the command line.
- Compile and execute a program.
- Submit your work.

## Assignment
### exercise1
1. create a file named main.cpp and the sample output of it is:
```
This is my first lab exercise!
```
2. create a file named Makefile and run it by typing the command 'make', then you can run the program by typing the name of your program, like:
```
./ex1
```

### exercise2
1. create a file named main.cpp and the sample output of it is:
```
My name is Xiangyu.
I am an EE major.
My hobbies are: 
     Table tennis
     Reading
Goodbye
```
2. create a file named Makefile and run it by typing the command 'make', then you can run the program by typing the name of your program, like:
```
./ex2
```

Your submission should be a file like Smith-123456-Lab-01.tar.gz. And the directories and files in it should be like this:
```
exercise1: main.cpp, Makefile
exercise2: main.cpp, Makefile
```
#### Only .cpp and Makefile are included, no .o files. 


## Main commands you need to get familiar with in lab 01:
```shell
cd ~
mkdir EECS_168/Lab1/exercise1 -p
cd EECS_168/Lab1/exercise1
touch main.cpp
gedit main.cpp &
g++ main.cpp -o ex1
./ex1
touch Makefile
gedit Makefile &
make
tar -cvzf Smith-123456-Lab-01.tar.gz Smith-123456-Lab-01
tar -tvzf Smith-123456-Lab-01.tar.gz
```

## FAQ:
1. Whether my files will be saved in my account if I log out or change a computer in the lab?
* A: Yes, all of your files will be saved to your EECS account. You can see them when you login next time.
2. Get an "unauthorized ..." error when creating a file.
+ A: You have no authorization to edit the current directory. Use the command "cd ~" to go to the **home directory**.
3. What is Makefile?
- A: A series of commands and rules to avoid retyping the same commands again and agian after making some changes. You only need to type 'make' command to generate a new executable program after some changes to your source files.
4. Why do we use command lines instead of GUI?
- A: https://wiki.ittc.ku.edu/ittc/images/9/99/Cmdline_instructions.pdf
