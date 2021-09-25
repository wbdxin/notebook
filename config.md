# 环境描述  
1. vscode  
2. git   
3. github

# install  
    vscode  
        ->使用chocolatey  
        ->https://chocolatey.org/  
        ->choco install vscode
        -->choco update all -y
    git  
        ->choco install git  

# config  
    git:  
        创建本地目录:  
        mkdir "directory_name"  
        cd "directory_name"
        git init  
        
        配置通用参数:用户名/邮箱  
        $ git config --global user.name "Your Name"  
        $ git config --global user.email "Your email"  

        创建ssh key  
        $ ssh-keygen -t rsa -C "Your email"
        打开所创建的id_ras.pub,复制所有内容,并添加到github [github->setting->ssh and gpg keys]

        