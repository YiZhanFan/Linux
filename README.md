# 准备工作

安装 windows 管理工具 chocolatey，通过 chocolatey 管理软件

-   choco install git
-   choco install tortoisegit
-   choco install vscode
    -   安装 Chinese (Simplified) Language Pack 
    -   安装 markdown all in one
    -   安装 markdown preview enhanced

# 配置公私钥对

1. 生成公私钥对
   
   要使用 git 来 clone 作业仓库，首先要使用之前提到的 puttygen.exe 生成公私钥对来生成公私钥对。
   
   点击 Generate 并持续晃动鼠标，即可完成公私钥生成。

2. 将公钥保存到远程仓库
   
   1. 打开 Github 并登录自己账户
   2. 点击右上角个人头像，在弹出的下拉菜单中选择 Settings 进入设置页面
   3. 点击设置 SSH and GPG keys 然后
   4. 点击 New SSH key 来新建一个 SSH key
   5. 在新建 SSH key 的页面将刚才用 puttygen 生成并复制了的文本形式公钥 (以 ssh-rsa 开头的一大串字符) 贴在 Key 对应区域，并在 Title 处填入自己喜欢的名字保存即可

3. 将私钥保存到本地
   puttygen.exe 的界面中点 Save private key 并确定不用密码保护后，选择一个路径存放自己的私钥。

# clone 仓库

1. 新建文件夹，选中文件夹右键（或进入文件夹，空白处点右键），在弹出的系统右键菜单中选择 Git Clone... 选项，会自动弹出 clone 界面
   
2. URL 是个人作业仓库的 Clone with SSH 链接，Directory 是你要存放代码的本地路径，Load Putty Key 则是私钥的路径（注：私钥必须是与刚才在 Github 账号中粘贴的公钥是同时生成的才能认证成功），点 OK 就会把作业仓库 clone 到本地





