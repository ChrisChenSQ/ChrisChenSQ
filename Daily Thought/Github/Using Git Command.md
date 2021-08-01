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

