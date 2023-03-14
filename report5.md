# CSE 15L Report 5

Throughout the entirety of this course, there have been multiple labs that I enjoyed participating in. If there had to be one specific lab report that I could choose, I would choose with most recent lab report. In Lab Report 4, we discussed how we could make edits in different files with the `nano` command. This command is very helpful because it allows us to do all our work and edits straight from the terminal instead of a software like VS Code.

In this lab, I was able to incorporate the skills I have used from the previous weeks to help me do this lab significantly faster. For example, the `<tab>` button is extremely helpful for autocompleting any command or file that you are trying to type. It makes working in your terminal a whole lot faster. I wish I had practiced this before my first skill demo because it would have made my time a lot better and help me get that high pass. Another example of a command that helped me work faster was the `<ctrl> + R` command. This command allows the programmer to search for anything that was previously typed in the terminal and you can retype it instead of having to use the arrow keys to go back and forth from a command you ran a while ago. For instance, for the very beggining of Lab Report 4, the first thing I had to do was sign into my ssh account. However, since I haven't signed into my account in a while, I could use the`<ctrl> + R` command and type the letter `s`. This will automatically have my ssh account pop up directly in the terminal. Then all I would have to do is click `<enter>`. This will automatocally sign me into my ssh account. 

![image](https://user-images.githubusercontent.com/122493451/221750669-ce4cc351-4503-4bc3-912f-c4b0d5bf92bb.png)

Luckily, we had previously learned how to take off our password through one of the labs. However, we never learned how to put our passwords back onto our account. This can create a security issue due to the fact that other students can long into our ssh account without a password. I would love to learn how I could readd a password or maybe even change the password through the terminal if that's possible. 

When I had logged into my ssh account, the first command I usually run is the `ls` command to check every folder that is in my server. Now we need to make sure that we clone our repository that was given to us. We do this with the `git clone` command. Then I copied and pasted the link from the github repository into the terminal and clicked `<enter>` which created a new directory. The next command would then be `cd ` along with the name of the directory which is "lab07". However, I only need to click `l` and `<tab>` which would completely autocomplete to the only directory that starts with "l". We then click `<enter>` to run the command. 
![image](https://user-images.githubusercontent.com/122493451/221752718-a644c7ae-2942-4914-a695-ca90d193b9d6.png)\
Now we check that all the files are there with the `ls` command. Once we confirm it, we compile and run our testers to find out where the issue is located. To compile, all I did was click the up arrow eleven times since I had called the command previously when I was during my first run. I then would click enter. I would then do the exact same thing to run it: Up Arrow 11x and `<enter>`. By doing this, we can see the error that we get which is: 

![image](https://user-images.githubusercontent.com/122493451/221755134-7f629056-ce05-4a6e-b84e-68e4a5f0f722.png)

Now that I am looking back at it, I wonder if the `<ctrl> + R` command would work to find the line to compile the tests. If I could do one thing differently, it would be that. Though I do not know if it would work since it is on a remote server, but there is no harm in trying. I would do the exact same thing with running the tester as well.

After this step, we must edit our tester file to get rid of this error. To edit this file, I typed, `nano L` + `<tab>` + `T` + `<tab>` + `j` + `<tab>` + `<enter>`. This sequence for typing makes it easier to type the command which gives us `nano ListExamplesTests.java`. When we click enter, we get greeted with this screen. 

![image](https://user-images.githubusercontent.com/122493451/221758516-b2d48b3c-4e65-42cc-a452-17950593a841.png)

This is where the nano command becomes so useful. With the nano command, we can edit these files directly from the terminal. Usually, we would have to open up VS Code and change everything on there. However, I believe it is easier since all our work is in the terminal already. There is no point in opening another window when we can change it directly in the terminal.

Once we have the nano command running, we must make a change in the file. We can search the thing we want to edit. If we type `<ctrl> + W` along with `l1` and `<enter>`, it will give us the first appearance of l1. We want the last appearance of it though, so we would have to type `<ctrl> + W` and `<enter>` exactly three more times. Now we want to switch l1 and l2 together. We click the right arrow key twice and hit delete and the number 2. Now we click the right arrow key four times, delete, and the number 1. This will switch l1 and l2 position.

Now to save the changes and exit, we click `<ctrl> + O`, `<enter>`, and `<ctrl> + X`. Once this is over, we can recompile and run ListExamplesTests.java. Since we had compiled and ran the tests earlier, we would just have to click the up arrow 3 times and `<enter>`. When we do this twice, we can see that the tests now pass. The screen should look like this:

![image](https://user-images.githubusercontent.com/122493451/221761921-04e5291e-7282-4dcf-9dd7-457d102e9438.png)

Now that we have our changes made on our ssh account. We can recompile and rerun our tester to see if the problem still occurs. We should notice that the tests pass successfully. This means we can now save and push our changes into github. We can do this by typing `git add L` + `<tab>` + `T` + `<tab>` + `j` + `<tab>` + `<enter>`. Then we type `git commit -m 'updated'` + `<enter>`. After that, we type, `git branch -M main` + `<enter>`. Finally we type, `git push -u origin main` + `<enter>`. All of this will commit and push our changes into github. Our terminal should look something like: 

![image](https://user-images.githubusercontent.com/122493451/221764494-87f6bb65-75c8-4171-aa96-4e6c3aae89f7.png)

When we then go into github, we can see that our file gets changed and the git ID is the same as the one we see in our terminal. We can see the change we made as well:

![image](https://user-images.githubusercontent.com/122493451/221764835-9cba0141-8e0a-43fe-ba4d-ee3775ad7f0b.png)

Throughout all of lab 4, I am trying my best to run these commands as efficiently and quickly as possible because I want to be able to get a High Pass on Skill Demo 2 which means I must practice from now. All these labs are great practice. Throughout these labs, I make sure to encorporate the autofill function in the terminal by clicking `<tab>`. I also want to ensure accuracy so I was check what directory I am in and what files are in my directory. I do this with the `pwd` command and the `ls` command respectively. I also ensure that I save time by running commands like `<ctrl> + R` so I do not have to write out tedious long commands in my terminal. Overall, these tips and tricks were very helpful in getting Lab Report done quickly and efficiently.
