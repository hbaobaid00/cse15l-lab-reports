# CSE 15 Lab Report 3

The "find" command in bash has lots of different command line options. One of the ways we can use bash in our command
is like this:

find -name "filename"

We can replace filename with anything we want to search for. If we wanted to only search for textfiles, we can replace filename with "*.txt". This is a common command line that we have used in our skill demo that allows us to find all the files that have a .txt file in them. Of course, the .txt can be replaced with other words in the file to help you look for a more specific file. Here is an example of me using this command to search the folder "written_2" that was given to us during the practice skill demo:\
![image](https://user-images.githubusercontent.com/122493451/218655863-a0dce52d-1739-4713-9d50-018930e9e7a2.png)\
Of course, there are more files, but I could not fit them all into one screenshot.\
Here is another example but this time I search for files that have the word "Vallarata" in them.\
![image](https://user-images.githubusercontent.com/122493451/218657327-af3f1edc-40b1-48aa-9b06-730d4263b276.png)\
Here we can see that the command returns every file with the string that contains "Vallarta" which can be extremely helpful.\
We can also search for files based on modification times like this: 

find -mtime -30 -name "*.txt"

which will tell you all the files that have been modified in the last thirty days. When I use this command, all the files are returned because I saved the folders for the practice skill demo about a week ago and never modified anything.\
![image](https://user-images.githubusercontent.com/122493451/218661065-35ce3bf9-3b8a-4e96-b87d-1672508d9a98.png)\
We can also use a "+" sign in front of the modication number to indicate the terminal to look for a file that was modified over that amount of time. So if I want to look for a file that was edited over a month ago, I would just simply write:

find -mtime +30 -name "*.txt"

When I do this, I do not get an output since everything was done within the past month.\
![image](https://user-images.githubusercontent.com/122493451/218662864-f31b9432-e1c8-45d6-b0e9-41615a139617.png)

Another thing we can do with the find command is look with files with a certain size. We do this by writing:

find -size +1M

The one can be replaced with any integer that represents the targetted file size. I used one because most files in the skill demo were text files which do not take that much space and were below 1 megabyte:
![image](https://user-images.githubusercontent.com/122493451/218667121-ac1e7f00-8bc8-4d92-aabc-1de5f2928e15.png)\
When I use 0 instead of 1, it outputs all the text files including more:

![image](https://user-images.githubusercontent.com/122493451/218667569-38ffbaf4-91b5-4f7d-bdfe-112810b22cf2.png)

Finally, another command line that goes with find would be:

find -type ...

After that command, you must type a corresponding letter. For example, if you type d, it will give you the corresponding directories like this:

![image](https://user-images.githubusercontent.com/122493451/218670134-2c243efd-379c-4ea8-86cf-e32b7666ffdc.png)

This is just one possibility of many others. Another letter you can type could be f. This would just give you all the possible files in the directory you are in.

![image](https://user-images.githubusercontent.com/122493451/218671561-fbed499a-45d4-481c-b3dd-8bdc8eb53476.png)

There are a lot more things you can do with the find command but these are just a few options from my research.

Resource: ChatGPT and VSCode
