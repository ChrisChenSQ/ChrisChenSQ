# Using Git Command

To upload a new file to a new repository on GitHub,

First, create a README.md file using the command,

```
echo "# Repository Name" >> README.md
```



 Then, initial the entire file using the command,

```
git init
```



Add files that you want to push to the repository. If all the files need to be pushed, then use * to represent.

```
git add *
```



Commit the push using the command,

```
git commit -m "first commit"
```



Add branch to the repository, using the command,

```
git branch -M main
```



Add the repository path using the ssh or HTML link, use the command,

```
git remote add origin xxxx
```

replace xxxx with the link.



Finally, push it to GitHub, use the command,

```
git push -u origin main
```



## Some common Git command

after you change some file locally, you could use the command,

```
git status
```

to check the status of the whole local repository. The file name in red means that this file is changed and it is not committed. If the file name is green means that the file is committed and is ready to be pushed.



To check the difference of change, you could use the command,

```
git diff
```

to check the difference between the previous version and the current version.
