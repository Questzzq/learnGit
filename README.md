# Record some common operations on GitHub
---
### Workfolw
+ Your **local-repository** consists of three "trees" maintained by git. the first one is your **Working Directory** which holds the actual files. the second one is **the Index** which acts as a staging area and finally **the HEAD** which points to the last commit you've made.
### add & commit
+ You can propose changes (add it to **the Index**) using
**`git add <filename>`** or **`git add *`**.
This is the first step in the basic git workflow. To actually commit these changes use **`git commit -m "Commit message"`**
Now the file is committed to **the HEAD**, but not in your remote repository yet.
### pushing changes
+ Your changes are now in the HEAD of your local working copy. To send those changes to your remote repository, execute 
git push origin master
Change master to whatever branch you want to push your changes to. 
+ If you have not cloned an existing repository and want to connect your repository to a remote server, you need to add it with
git remote add origin <server>
Now you are able to push your changes to the selected remote server.
---
1. Go to your Github website homepage and new a **remote-repopsitory**.
2. Go to a diectory, open a shell and type **`mkdir local-repository`**.
3. **`cd local-repository`**.
4. **`touch README.md`**.
5. **`vim README.md`** and write something to about your project, save and exit.
6. type **`git init`** to initial your **local-repository**, don't foget a keypoint: type **`git config user.email "youremail@xxx.com"`**, and type **`git config user.name "your_Github_Name"`**. These two statements declare the identity and the operation object of the commands.
7. Now supposed you want to upload a **main.cpp** to your **remote-repository**.
8. **`touch main.cpp`**.
9. **`vim main.cpp`**, save and exit.
10. Note that now **README.md** and **main.cpp** just exist in  **Working Directory**, to commit them to your **remote-repoditory**, you first need to push them into **the Index**.   
11. use **`git add File-Name/Directory-Name`** to have your file/directory into the **cache-area**. In this example, we type **`git add README.md`** and **`git add main.cpp`** or just type **`git add *`**.
12. Now type **`git commit -m "Commit Message"`** to commit **main.cpp** and **README.md** to **the HEAD**. 
13. Now you can push the files from **the HEAD** to your **remote repository**, you just need to type **`git push -u origin master`**.
14. Then according to the feedback in the shell, completet them and work done.
