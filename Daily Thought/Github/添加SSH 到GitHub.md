# 添加SSH 到GitHub

首先添加user name和email。user name就是如果你要push的话显示的user name，email就是你的github账户email。`

```stylus
git config --global user.name "xxx"
git config --global user.email "xxx@yeah.net"
```

生成密钥：

```
ssh-keygen -t rsa -C "{{ github email }}"
```

如果不需要ssh密码的话，连续三个`enter`键。

跑完这个命令后会获得2个文件。`id_rsa` & `id_rsa.pub`

如果你是windows，打开这个文件路径`C:\Users\{{ computer name }}\.ssh`。打开`id_rsa.pub`文件，把里面的东西全部复制下来。这个就是你的电脑的ssh key。

下一步就是添加ssh key到github你的账户里。
