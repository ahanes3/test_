# Test Git Repository 

**Author:** Alex Hanes  
**Date:** June 11, 2024 (T)  


This is a test repository to see how you create a `git` project.  
# Steps 

1. Create a new directory 
2. Initialize a git repository using `git init` 
3. 

# Useful Commands 

`git init`  
> Create a new git repository 

`git status`  
> Very useful.

`git add <file>`  
> Add a file to the staging area  

`git add .` 
> Add all files to the staging area  

`git branch -m <name>`  
> .

`git commit -m "<commit-message>"` 
> `m` stands for message  
> I think the commit message has 50 char. maximum  

`git restore <file> ...` 
> .




# Git Branch: Make Changes to Repository without Modifying the Main Branch 

`git checkout -b "<branch-name>"` 
> TBD.  

To go back to the master branch: 
`git checkout master`  

We added some documentation notes to the `readme.md` file in the `master` branch **after** we made the `branch-first` branch. When we navigated to the `branch-first` branch, these changes were not reflected in the `readme.md` file. Likewise, when we initially made the `branch-first` branch, the `readme.md` file was updated and a `main.py` file was created, but these changes were not reflected in the `master` branch. Now, we need to merge all changes.  

I will do this in the `branch-first` branch:  

`git merge master`  

Finally, once this is done, I will navigate back to the `master` branch:  

`git checkout master`  

Then merge the `branch-first` branch with the `master` branch (if I am happy with it):  

`git merge branch-first`  

Now, I should see two files when I type `ls`: 
- `readme.md` 
- `main.py` 




# Terms 

Staging Area   
Repository  
Branch  
Fork  
Clone  