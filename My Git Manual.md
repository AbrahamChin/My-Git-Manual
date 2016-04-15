# How to use Git
### 1. Creating a repository 
1.1 Create a folder that you will be working on, let it be named as **git-test**. Right click "**Git Create repositoty here...**" at the folder .
1.2 Git Init window pops up to inquire your option of whether `Make it Bare (No working directories)` or not. If you plan to work inside the folder, uncheck the option, the folder will work a bit like a user. Or else check it, the folder will work as a local server to accept **pushes**, in this case, you'd better append the folder name with `.git` for easier recognition.
1.3 Click **OK**, and a message follows saying "Initialized empty Git repository in `D:\Abraham\My Git\git-tset`".
1.4 Create a text file `hello.txt`, type in `hello world`. Now you have a new file in the folder (repo), then you right click `hello.txt`, select "**ToitorseGit->Add...**", the file will be added to **Git stage** from your **working directories**.
1.5 Right click `hello.txt`, select **Git commit -> "master"...**, enter into message why changes were made, and **Commit**. The created file is moved from **Git Stage** to **Master Branch**.
1.6 Now you can create more files within the folder or working directory, and commit to master branch.

### 2. Cloning a project to local repository
2.1 **Run TortoiseGit PuTTYgen** to generate SSH Key, and save **private key** on a folder where you could find it easily.
2.2 Copy **SSH clone URL** from project you are interested in.
2.3 Right click blank area, select **Git clone...**, 
enter URL by pasting from clipboard. Directory is automatically created in the folder where you right clicked. And **load Putty Key** that you saved. Click **OK**.
2.4 Now a folder named "My-Git-Manual" is created. You can see default files .gitignore and .gitattributes in the folder.
2.5 Now you can create files in the folder as steps decribed by 1.4 and 1.5.
2.6 If you ensure all your commits in the default Master Branch are ready to push to remote server, you can right click the foled "My-Git-Manual", and select "TortoiseGit->Push..." and OK. The modification will be updated to the branch on GitHub.


### 3. Setting branches
3.1 Clone two identical folders from GitHub. One is named as "My-Git-Manual", the other is "My-Git-Manual-Branch". Both folder are on **Master Branch**. (You can think it as created for two users who work on this project simultaneously with default branch Master, from GitHub view, Master is the production line, you need create new branch off the production line for specific purpose, such as, debug, features).
3.2 Right click "My-Git-Manual-Branch", select "**TortoiseGit->Create Branch...**", enter Branch name, like "debug", then click **OK**.
3.3 Right click "My-Git-Manual-Branch", select "**TortoiseGit->Switch/Checkout...**", switch to "debug", then click **OK**.
3.4 Now right click "My-Git-Manual-Branch", **Git Commit->"debug"** is shown instead to master branch.
3.5 Now you could push it to remote server.