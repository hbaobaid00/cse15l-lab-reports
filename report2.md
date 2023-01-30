# CSE 15L Lab Report 2
For today's lab report, we were required to create a web server that would return strings on the screen based on what is entered in the URL. I was able to use previous resources to help me create this web server. The code for my web server looks like this:
![StringServer5](https://user-images.githubusercontent.com/122493451/215411523-0307e03b-8ca3-4f75-91a9-eaba03bf05d2.png)\
I first had imported some libraries that are a part of Java. These libraries help me create methods to run a server. I created a handleRequest method which basically helped break the url down and would return the message of the string. I had sure to make the message was a static variable so it would keep the message on the screen if you typed a different url. I also used the Server class that was given to us when we created local host servers in one of the lab. It was extremely useful, especially when making your own server. 

Here are what the results look like for the code:\
![StringServer](https://user-images.githubusercontent.com/122493451/215415650-aaba67a4-6087-47aa-828d-f3ea6734b590.png)
![StringServer2](https://user-images.githubusercontent.com/122493451/215415668-05ab21f1-2003-4fab-ba40-73c6a6296278.png)
![StringServer4](https://user-images.githubusercontent.com/122493451/215415760-0b5fc190-6ce8-460e-8483-84065af07cb4.png)\
If the path is not typed out as intended, there will be a 404 error not found that is shown on the screen. However, when you do type the path correctly. Your message will be shown on the screen and a new line will be entered for the next message. If you re-enter the same path in the URL, your message will be printed twice. It will keep printing the same message repeatedly. If you do not type a path at all. A 404 error message will be seen on the screen just like when you type the path incorrectly. 


