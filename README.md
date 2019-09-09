# EECS168-Lab-Xiangyu
This repository is used to post some information about the labs and FAQ. If you have any questions, you could either ask in the "Issues" section above (I will answer when I see them and everybody else can answer if you want to. Besides this, you can search the questions here before asking to get your answer quickly.) or email it to me. 

## Some tips:
1. Use your keyboard instead of your mouse. (Use commands 'cp, mv, cd, pwd...' instead of right-clicking on your mouse)
2. A useful blind type training website: https://www.keybr.com. 
3. Use the up arrow to get your previous commands.
4. Use the Tab key to complete the filename or directory automatically.

## Assignment Due time:
Due for 8-9:50 Monday lab is Sunday (11:59 p.m.);
Due for 8-9:50 Friday lab is next Thurday (11:59 p.m.);

## Assignment Submission:
1. create an archive of your exercises:
```
tar -cvzf Smith-123456-Lab-01.tar.gz Smith-123456-Lab-01
```
2. Email this .tar.gz file to me with a subject like:
```
[EECS168] Lab01
```
## How to create a Makefile
```
touch Makefile
gedit Makefile
```
A Makefile should be like this:
```
target: prerequisites
[tab]command
```
An example is:
```
HelloWorld: main.o
	g++ -std=c++11 -g -Wall main.o -o HelloWorld

main.o: main.cpp
	g++ -std=c++11 -g -Wall -c main.cpp

clean: 
	rm *.o HelloWorld
```
And then run your Makefile to make sure it is executable.
```
make
```
After this, an executable will be generated. (The last target "clean" and its command will not be run when typing "make". To execute the clean command, you need to use the command "make clean".) Run it:
```
./HelloWorld
```
Then, to submit your assignment and also make your files neat, you should clean all .o files and executable files. Use the command:
```
make clean
```

