# CSE 15L Report 4

Starting off with the first step, the keys I used to sign into my ssh account are as follows: `<ctrl> + R`, `s`, and `<enter>`. The first two keys allow me to find previous commands that were typed in the terminal. After clicking `Ctrl + R` along with `s`, my terminal looks like this:\
![image](https://user-images.githubusercontent.com/122493451/221750669-ce4cc351-4503-4bc3-912f-c4b0d5bf92bb.png)\
Once I click enter, I become logged into my ssh account where I can move on to the next steps.

When it comes to the next step for cloning the repository, the command that was typed into the terminal was, `git clone ` along with a left click on the terminal. When I left click, it pastes whatever was copied and in this case, I had copied the repository from git hub. After this, I clicked `<enter>` which gave me this screen: 
![image](https://user-images.githubusercontent.com/122493451/221752718-a644c7ae-2942-4914-a695-ca90d193b9d6.png)\
This means that the repository was cloned successfully, so I can move onto the next step. 

For the next step, I had to make sure that I changed my directory into the repository that we just cloned so I typed `cd l`, `<tab>`, and `<enter>`. By clicking tab, it would autocomplete to the directory I need because it is the only directory in the account that starts with "l". Once I am in the directory, I would now need to compile and run the files in the directory. To compile, all I did was click the up arrow eleven times since I had called the command previously when I was during my first run. I then would click enter. I would then do the exact same thing to run it: Up Arrow 11x and `<enter>`. By doing this, we can see the error that we get which is: 
![image](https://user-images.githubusercontent.com/122493451/221755134-7f629056-ce05-4a6e-b84e-68e4a5f0f722.png)\

After this step, we must edit our tester file to get rid of this error. To edit this file, I typed, `nano L` + `<tab>` + `T` + `<tab>` + `j` + `<tab>` + `<enter>`. This sequence for typing makes it easier to type the command which gives us `nano ListExamplesTests.java`. When we click enter, we get greeted with this screen. 

![image](https://user-images.githubusercontent.com/122493451/221758516-b2d48b3c-4e65-42cc-a452-17950593a841.png)

Now the edit we have to make is on the last line. We can search the thing we want to edit. If we type `<ctrl> + W` along with `l1` and `<enter>`, it will give us the first appearance of l1. We want the last appearance of it though, so we would have to type `<ctrl> + W` and `<enter>` exactly three more times. Now we want to switch l1 and l2 together. We click the right arrow key twice and hit delete and the number 2. Now we click the right arrow key four times, delete, and the number 1. This will switch l1 and l2 position.

Now to save the changes and exit, we click `<ctrl> + O`, `<enter>`, and `<ctrl> + X`. Once this is over, we can recompile and run ListExamplesTests.java. Since we had compiled and ran the tests earlier, we would just have to click the up arrow 3 times and `<enter>`. When we do this twice, we can see that the tests now pass. The screen should look like this:

![image](https://user-images.githubusercontent.com/122493451/221761921-04e5291e-7282-4dcf-9dd7-457d102e9438.png)

Now for the final step, we must push our saved changes into github. We can do this by typing `git add L` + `<tab>` + `T` + `<tab>` + `j` + `<tab>` + `<enter>`. Then we type `git commit -m 'updated'` + `<enter>`. After that, we type, `git branch -M main` + `<enter>`. Finally we type, `git push -u origin main` + `<enter>`. All of this will commit and push our changes into github. Our terminal should look something like: 

![image](https://user-images.githubusercontent.com/122493451/221764494-87f6bb65-75c8-4171-aa96-4e6c3aae89f7.png)

When we then go into github, we can see that our file gets changed and the git ID is the same as the one we see in our terminal. We can see the change we made as well:
![image](https://user-images.githubusercontent.com/122493451/221764835-9cba0141-8e0a-43fe-ba4d-ee3775ad7f0b.png)

This completes all of our steps for this lab.
