# Git & GitHub

## Step 1: Download Git
To start Git and GitHub.
1. Create a GitHub account.
2. Download and Install Git in desktop.

## Step 2: Configuring Git
1. Then open Git Bash and login by using user name and email.
2. We have two types of configuration * Global Level  * Local Level
3. Basically we use Global level which control our whole system changes.
4. When we open Git Bash we get this line of code in our Git Bash terminal ``` ALOK@DESKTOP-D41A0U8 MINGW64 ~ ```
5. This ```~``` indicate's that we are inside Root Directory user.
6. For Checking the version for our Git which we install type ``` git --version ```
```
    $ git --version
    git version 2.44.0.windows.1
```
7. For Configuratio we have to give user Name & user E-mail 
8. For user name type    ```  git config --global user.name "Alokkumar-8467" ```
9. In User Name we will type the name that we took while creating the GitHub account.
10. For email type  ```  git config --global user.email "alokkumarcse01@gmail.com" ```
11. To know what are the things we config in Git For that type  ``` git config --list ```
```
    ALOK@DESKTOP-D41A0U8 MINGW64 ~ $ git config --list
    user.name=Alokkumar-8467
    user.email=alokkumarcse01@gmail.com
```
> We can use Git command inside Git Bash OR we can also use Code Editor for this work.
> It's better to use Code Editor so that at the same time we can check our program code and also use Git commands on it at same time.

## Some basic Command
###### cd
> For changing directory form one to another 
###### ls 
> all list of file inside that particular folder
###### ls -a
> it's shows hidden file in that folder
###### cd .. 
>move out from that directory
#### mkdir 
>make new directory
> ` mkdir "FolderName" `

## Some basic Git Commands

### Clone & Status

#### Clone : 
> Cloning a repository on our local machine.
> git clone <-some project link which is uploaded on GitHub ->

``` git clone https://github.com/Alokkumar-8467/Git-GitHub.git  ```
OR

git clone -b <branchName> <project github link>

` git clone -b 18.Delete-Task-By-Login-User https://github.com/Alokkumar-8467/Next.js.git`

1. We simply open any project which uploaded on GitHub.
2. Click on Code button which is green in color.
3. It show's many option, Click on HTTPS link and copy and paste like that ``` git clone https://github.com/Alokkumar-8467/Git-GitHub.git  ```
4. That Code is copy in your Code Editor and we can make changes on them.

#### Status : 

>display the status of the code
> ``` git status ```

Git has four types of Status.
1. Untracked : new file that git does't yet track
2. Modified : changed
3. Satged : file is ready to be commited
4. Unmodified : unchanged
```
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html
        total.html

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html
        new file:   total.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html
```

#### Add & Commit

#### Add :

1. add - adds new or changed files in your working directory to the Git staging area.
2.  ` git add ` For one file
3.  ` git add . ` For add more than one file at a time

#### Commit :

1. it is the record of change
2.  ` git commit -m "some message" `
```
[main (root-commit) 674c27d] Work done
2 files changed, 22 insertions(+)
create mode 100644 index.html
create mode 100644 total.html
```
4. After commit it shows nothing to commit
```
On branch main
nothing to commit, working tree clean
```
#### Push Command

1. Push - upload local repo content to remote repo
` git push -u origin main `
2. If it's not work then use ` git push --set-upstream origin main -f `

#### Init Command
> init - used to create a new git repo
1. `git init` 
2. `git remote add origin` 
3. `git remote -v (to verify remote)`
4. `git branch (to check branch)`
5. `git branch -M main (to rememe branch to main)`

#### Branch Commands

1. `git branch ` to check branch
2. `git branch -M <NewBranchName>` to remane branch
3. `git checkout <Name of that branch to which we want to Navigate>` to navigate
4. `git checkout -b <Name of that branch to which we want to Create>` to create new branch
5. `git branch -d <Name of that branch to which we want to Delete>` to delete branch



