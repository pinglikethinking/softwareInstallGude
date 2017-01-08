# softwareInstallGude
reinstall the system,and then reinstall all. so write this down

### node&&npm install(> http://m.blog.csdn.net/article/details?id=51160334)

1.https://nodejs.org/

set path:F:\nodejs

win+r---cmd:node -v---npm -v


2.config enviroment

```

1) config --- global cache

> 我们要先配置npm的全局模块的存放路径以及cache的路径

npm config set prefix "C:\Program Files\nodejs\node_global"

npm config set cache "C:\Program Files\nodejs\node_cache"

2)test---global cache

cmd:npm install express -g

3)close cmd--open mycomputer 

> “我的电脑”右键“属性”-“高级系统设置”-“高级”-“环境变量”

program path---add NODE_PATH:F:\nodejs\node_global\node_modules

user path---change PATH:F:\nodejs\node_global\

> 由于改变了module的默认地址，所以上面的用户变量都要跟着改变一下（用户变量”PATH”修改为“F:\nodejs\node_global\”），要不使用module的时候会导致输入命令出现“xxx不是内部或外部命令，也不是可运行的程序或批处理文件”这个错误

```


### git install(git bash,git gui)

https://git-for-windows.github.io

test----cmd : git bash

set git username&useremail:

```

$ git config --global user.name "Your Name"

$ git config --global user.email "email@example.com"

```

produce ssh:

```
first check if the ssh is right:

ssh -T git@github.com

hi...--so succeed

OR walk the follow:

1)check:

cd ~/.ssh

"no such file..."--then 3,OR 2 backup copy

2)backup copy:

mkdir key_backup mv id_isa* key_backup

3)new key:

$ ssh-keygen -t rsa -C "pinglikethinking@gmail.com"

...three enter

4)push ssh:

/users/your_user_directory/.ssh----open id_rsa.pub----ctrl+c

open github.com/setttings/ssh---add ssh key----ctrl+v

5) check:

the same to 1)
```


### webStorm install

http://www.jetbrains.com/webstorm/

search license server one:http://114.215.133.70:41017

