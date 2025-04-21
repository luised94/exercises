
# exercises
## Introduction
This repository contains exercises for the [performance-aware programming](https://www.computerenhance.com/p/table-of-contents) course. I may add exercises related to other textbook or courses but, for now, there are only the ones for computer enhance.
The computer_enhance repository is present as a submodule.

## Setting up computer_enhance submodule
To setup the computer_enhance repository as a submodule, perform the following steps:
1) Create a repository on github or wherever you host your repository.
2) Initialize the repository locally.
```{bash}
mkdir exercises
cd exercise
git init
touch README.md
git add .
git commit -m "First commit"
git remote add origin https://github.com/luised94/exercises.git
git push -u origin main
# enter username and password
```

3) Set the computer enhance as the submodule
```{bash}
git submodule add https://github.com/cmuratori/computer_enhance.git
git commit -m "feat(submodule): Add computer_enhance as a submodule"
git push origin main
```

4) Use git pull while inside the submodule directory to update the directory then update your repository to tell it the new commit of the submodule.
