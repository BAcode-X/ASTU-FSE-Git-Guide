# ASTU-FSE-Git-Guide
### A simple guide for learning Git

Before jumping into the code, let's first try to cover some common <b> terminologies </b> related to version control.

#### 1. Version Control System : 
allows you to revert files back to a previous state, revert the entire project back to a previous state, review changes made over time, see who last modified something that might be causing a problem, who introduced an issue and when, and more. 

#### 2. Repository :
directory that contains your project work which are used to communicate with Git. 
Repositories can exist either locally on your computer or as a remote copy on another computer.

#### 3. Commit :
Git thinks of its data like a set of snapshots of a mini file system.
Think of it as a save point during a video game.

#### 4. SHA :
A SHA is basically an ID number for each commit.
Ex. E2adf8ae3e2e4ed40add75cc44cf9d0a869afeb6

#### 5. Working Directory :
The files that you see in your computer's file system. 
When you open your project files up on a code editor, you're working with files in the Working Directory.

#### 6. Checkout :
When content in the repository has been copied to the Working Directory. It is possible to checkout many things from a repository; a file, a commit, a branch, etc.

#### 7. Staging Area :
You can think of the staging area as a prep table where Git will take the next commit. 
Files on the Staging Index are poised to be added to the repository.

#### 8. Branch :
it is when a new line of development is created that diverges from the main line of development. This alternative line of development can continue without altering the main line.

Git has three sections/areas

![](images/git_working_areas)

<em> Next, if you haven't installed git on your computer :</em>
#### For <b>windows</b> users install git bash from the following link : [Download Git](https://git-scm.com/downloads)
#### For <b>linux</b> users run the following command on the terminal : ```sudo apt-get install git```

##### To set the name and email for git to use when you commit use the following command :
```git config --global user.name "<your name>"```<br>
```git config --global user.email "<your email>"```

<em>Go to your github account and click the button <strong>New</strong> which is a button for creating a new repository. Then give it a name and click on the <strong>create repository</strong> button.</em>

##### Now copy the url and open the terminal and enter the following command
```git clone <url> [local dir name]```
<br>
This will create a directory named local dir name, containing a working copy of the files from the repo, and a **.git** directory

<em>Now you can start adding and commiting changes to your repository.</em>

##### Create a sample python file and name it test
```touch test.py```

##### To check about the status of your working directory, use the following command.
```git status```

<em>Go ahead and try the command now.
It will tell you that there is an untracked file and asks you to add the file using the **add** command.</em>

##### To add new files or changed files into the staging area use the add command
```git add <filename>``` in your case, 
```git add test.py```

<em>To add all new files you have created to the staging area, use the following command</em>

```git add .```

##### To commit the staged files, use the commit command followed by a message

```git commit -m "<message>"``` in your case, 
```git commit -m "added test.py"```

The message part is to describe what kind of change you have made to your directory or code.

<em> Now check the status of your working directory using the status command.</em><br>
You should be seeing **"nothing to commit, working directory clean"** message.
