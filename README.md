##

### 2.4

**首先来设置使用 Git 时的姓名和邮箱地址。名字请用英文输入。**
```
$ git config --global user.name "Firstname Lastname"
$ git config --global user.email "your_email@example.com"
```

这个命令，会在“~/.gitconfig”中以如下形式输出设置文件。
```
[user]
  name = Firstname Lastname
  email = your_email@example.com
```

**将 color.ui 设置为 auto 可以让命令的输出拥有更高的可读性。**
```
$ git config --global color.ui auto
```

**创建 SSH Key**
```
$ ssh-keygen -t rsa -C "your_email@example.com"
Generating public/private rsa key pair.
Enter file in which to save the key
(/Users/your_user_directory/.ssh/id_rsa): 按回车键
Enter passphrase (empty for no passphrase): 输入密码
Enter same passphrase again: 再次输入密码
...
Your identification has been saved in /Users/your_user_directory/.ssh/id_rsa.
Your public key has been saved in 
...
```
id_rsa 文件是私有密钥，id_rsa.pub 是公开密钥。
```
$ cat ~/.ssh/id_rsa.pub
```

```
git status
```






