# LinneaHubble.github.io

## To develop on local machine
```
docker run --rm -v `pwd`:/site -p 4000:4000 andredumas/github-pages serve --watch
```
The code for the advantage-seo.com website is in this folder on my laptop: LinneaHubble.github.io
Find it in Finder, right click, go to "Services" and "New iTerm2 window here". That will open the terminal in iTerm and I can do commands there. 

OR 

Open the program "Code" (Visual Studio Code) and the code is in there. 
In the terminal in Code, write "git pull"
Text about "reconsile divergent branches" can be ignored because it's not that complicated of an environment. 
Git pull checks if there are any updates to the files. In this case there are no updates so it doesn't say anything. 
You can type "clear" to get rid of the previous text. 

Start the Docker app. 

Then, in the terminal in Code, run this line
```
docker run --rm -v `pwd`:/site -p 4000:4000 andredumas/github-pages serve --watch
```

In the respons you get in the terminal, Open localhost under Server Adress: http://0.0.0.0:4000/ in a browser (Cmd+click to open).

Now you can start working. Edit your files and click "Save" in Code. You can see your changes at http://0.0.0.0:4000/. 

When you are done editing and have saved all your changes, go to the terminal in Code and write ctrl+C to stop the local Docker container from running. The page http://0.0.0.0:4000/ will no longer be working. 

In Code, go to Git Source Control in the left hand menu (it looks like a little branch with nodes) , and it will have the changed files so you can see what changes have been made. 
In the 3 dots on top, you have a menu with commands. You can do pull and push and other things from there, as well as in the terminal window. 

3 steps now:
- Stage changes (Plus sign)
- Commit changes
- Push changes

Stage changes (Plus sign)
Write a message to yourself (although it's public)

Commit - this means you're saving this change, along with the message, locally. The check mark on top means Commit.
Push - means you push your changes to the remote version (in this case it's deployment live to the web since I'm pushing to the master branch) on GitHub. 

Typing "git status" in the terminal will tell you the status of the files (same as you can see in the left hand panel). 

Typing "git push" (or use the 3 dot menu and choose "push") will push your changes to git and the website is updated. 

DONE!

## To do
Lots to do.

