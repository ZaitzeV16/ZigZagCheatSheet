# W01 - D03 - Git and Command Line
made by [<font color="SaddleBrown">***barna***</font> ***Barna***](https://github.com/bekobarna) <br/> <br/>

|[Command Line](#command-line)                                                          |[Git](#git---version-control-system)|
|:------------------------------------------------------------------------------------- |:---------------------------------- |
|[`cd` &ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;- change directory](#cd)   |[Repository](#repository)           |
|[`pwd` &ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;- print working directory](#pwd)|[`git init`](#git-init)             |
|[`ls` &ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;- list](#ls)               |[`git clone`](#git-clone)           |
|[`touch`](#touch)                                                                      |[`git status`](#git-status)         |
|[`mkdir`&ensp;&ensp;&ensp;&ensp;&ensp;&ensp; - make directory](#mkdir)                 |[`git diff`](#git-diff)             |
|[`cp` &ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;- copy](#cp)               |[`git add`](#git-add)               |
|[`mv` &ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;- move](#mv)               |[`git commit`](#git-commit)         |
|[`rm` &ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;- remove](#rm)             |[`git push`](#git-push)             |
|[`man` / `--help` - manual page](#man-and---help)                                      |[`git log`](#git-log)               |
|                                                                                       |[`git pull`](#git-pull)             |
|                                                                                       |[`.git`](#git)                      |
|                                                                                       |[`.gitignore`](#gitignore)          |

## Command Line
### `cd`
>  ***Change directory***

|Command   |Explanation              |
|:-------- |:----------------------- |
|`cd`      |Go to your root directory|
|`cd ..`   |Go 1 folder up           |
|`cd ../..`|Go 2 folder up           |

****

### `pwd`
> ***Show where you are, your current directory.***

****

### `ls`
|Command|Explanation                                            |
|:----- |:----------------------------------------------------- |
|`ls`   |List the contents of your current folder               |
|`ls -l`|List with details                                      |
|`ls -a`|List the hidden files (files starting with a .) as well|

****

### `touch`
>  ***Create a file.*** <br/>
>  + `touch example.txt`

****

### `mkdir`
>  ***Create a directory.***

****

### `cp`
> ***Copy files or directories.*** <br/>
> + `cp ‘what to copy’ ‘where to copy’`

****

### `mv`
> ***Move files or directories OR rename.*** <br/>
> + `mv ‘what to move‘ ‘where to move‘` <br/>
> + `mv ‘old name’ ‘new name’`

****

### `rm`
> ***Remove files or folders, it will only delete a directory, if it’s empty.***

|Command|Explanation                                                     |
|:----- |:-------------------------------------------------------------- |
|`rm -r`|Remove everything, even a non empty directory with it’s contents|
|`rm -v`|Removes a file and writes out what happened                     |

****

### `man` and `--help`
> + ***`man` won’t work on windows, only on linux and mac, you can view them [here](https://linux.die.net/man/)***
> + ***Write `--help` after a command, it will show the help page for it, but not for every command.*** <br/>

example: `mkdir --help`


## Git - Version control system
### Repository
> + ***the place where we store our code, like zigzag-syllabus, teaching-materials, your repositories***
>   + ***Local repository - it’s on your computer***
>   + ***Remote repository - on Github or on a similar site***

****

### `git init`
> ***Create an empty repository in your current folder.***

****

### `git clone`
> ***You clone an already existing repo from Github onto your computer.*** 

****

### `git status`
> ***Check the repo’s contents for any changes, which files are modified, are they in the staging area.***

****

### `git diff` 
> ***Shows what is different between a files current content and another one, check out the documentation for it, there are a lot of possibilities.***

****

### `git add`

|                          Command|                                        Explanation|
|:------------------------------- |:------------------------------------------------- |
|                        `git add`|stages the changes you made since your last git add|
|                      `git add .`|                          stages every modification|
|       `git add <file/directory>`|                     stages a chosen file/directory|
|`git add <file1> <file2> <file3>`|                              stages multiple files|


****

### `git commit` 
> ***Creates a commit from the staging area.***

****

### `git push`
> ***Pushes your commits to the connected remote repo (github).***

****

### `git log`
> ***Shows the commits.***

****

### `git pull`
> ***Get the changes from a remote repo and merges it into your local repo (makes the same).***

****

### `.git`
> ***Hidden folder, this makes a folder to a repository, if you delete it, you delete the repository.***

****

### `.gitignore`
> ***Write here, what you don’t want to involve in your commits, like generated files by your IDE or unnecessary files.***
