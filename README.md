# Education:

##
### There is a place where publishing study materials.

**before run (base settings):**

* git config --global user.email "you@mail.com"
* git config --global user.name "Your  Name"

**git main command:**

* git clone *../someproject.git*
* git status
* git add
* git commit -m "some comment"
* git push
* git pull
* git checkout
* git branch 

some important variation of commands:

* git add -A *(add all)* 
* git add --all *(add all)* 
* git add . *(add all)*
* git log
* git reset HEAD file *(to unstage)*
* git clone --mirror *../someproject.git*   **.git** *(clone all project with branches)*
* git config --bool core.bare false
* git reset --hard (grap all branches)
* git clone -b some_branch *../someproject.git*
* rm -dfr .git *(delete .git folder)*


**How delete file:**

1:

* delete file
* git add file (stage)
* git commit -m "delete file"

2:

* git rm file
* git commit -m "delete file"

reverse file:

* git reset HEAD file
* git checkout file

**Return Back and new Branches:**

* git checkout commit_hash
* git checkout master 
* git branch alternatebranche commit_hash
* git branch newname
* git branch -m oldname newname *(change branch name)*
* git branch -D deleted_branch *(delete)*
* git branch -a *(all branches, some can be absent on local machine)*
* git checkout -b branch_whatineed locationOriginOfBranch *(for example, I need download some branch from github)*


**Merge:**

* git merge somebranch *(merge with current)* 

