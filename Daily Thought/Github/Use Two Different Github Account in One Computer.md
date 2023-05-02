# Use Two Different Github Account in One Computer

This is a note for how to use a personal account and a work account on one computer. This is same for different platform.

## Step 1

Create separate ssh key pair using the code below

```ssh-keygen -t rsa -C "your email"```

Then use the code below to add both of the key pair to ssh

```ssh-add id-rsa```



## Step 2

Go to```.ssh``` file and create a new file called config using the code below

```touch config```



## Step 3

Inside the config, write the folloing code

```
Host personal  #This can be any name that you want
    HostName github.com
    User git
    IdentityFile ~/.ssh/id_rsa

Host work  # This can be any name that you want
    HostName github.com
    User git
    IdentityFile ~/.ssh/work

```



## Step 4

Change your remote repository to 

```
git@personal:[repository name]
# or
git@work:[repository name]
```

