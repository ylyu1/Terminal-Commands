# Setting Up a Remote Repository for a Local Git Project

## 1. Local Working Directory
Ensure you have a local working directory ready.

## 2. Create Remote Repository
Create a new repository on GitHub to track your local project.

## 3. Initialize Git
In your working directory, open a terminal and initialize Git. This creates a `.git` folder.

```sh
git init
```

## 4. Setup `.gitignore`
For files you don't want to track, create or edit a `.gitignore` file using VSCode.

```sh
code .gitignore
```
Inside the .gitignore file, list the files or directories you want to ignore. Here are some examples:

* For directories, add a trailing slash (/).
* For specific file types, use an asterisk (*) as a wildcard.

```
venv/
*.cpp
```
## 5. Track Files
Add all necessary files to Git.
``` sh
git add -A
```
## 6. Commit Changes
Stage and commit all files with a message. Use double quotes for messages.
``` sh
git commit -m "initial commit"
```
## 7. Add Remote Repository
Link your local repository to the remote one on GitHub. (Use remote repository URL)
```sh
git remote add origin http://...
```

## 8. Push to GitHub
Push your changes to the master branch on GitHub, setting up the upstream branch.
``` sh
git push -u origin master
```

