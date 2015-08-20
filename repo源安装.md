# 一、中科大repo源 #

首先备份CentOS-Base.repo


    mv /etc/yum.repos.d/CentOS-Base.repo /etc/yum.repos.d/CentOS-Base.repo.backup

下载对应版本的CentOS-Base.repo, 放入/etc/yum.repos.d/

这是CentOS 5的:
    
    wget http://lug.ustc.edu.cn/wiki/_export/code/mirrors/help/centos?codeblock=1
    
这是CentOS 6的:
    
    wget http://lug.ustc.edu.cn/wiki/_export/code/mirrors/help/centos?codeblock=2
    
下载完成后 ：


    运行yum makecache生成缓存 ，运行 yum update升级软件包
    
# 二、163 repo源 #

首先备份/etc/yum.repos.d/CentOS-Base.repo

    mv /etc/yum.repos.d/CentOS-Base.repo /etc/yum.repos.d/CentOS-Base.repo.backup

下载对应版本repo文件, 放入/etc/yum.repos.d/(操作前请做好相应备份)
    
   CentOS7
       
    wget -O /etc/yum.repos.d/CentOS-Base.repo http://mirrors.163.com/.help/CentOS7-Base-163.repo

CentOS6
    
    wget -O /etc/yum.repos.d/CentOS-Base.repo http://mirrors.163.com/.help/CentOS6-Base-163.repo
    
CentOS5

    wget -O /etc/yum.repos.d/CentOS-Base.repo http://mirrors.163.com/.help/CentOS5-Base-163.repo` 
    
运行以下命令生成缓存

    yum clean all
    yum makecache


# 三、阿里repo源 #

备份你的原镜像文件，以免出错后可以恢复。
    
    mv /etc/yum.repos.d/CentOS-Base.repo /etc/yum.repos.d/CentOS-Base.repo.backup

下载新的CentOS-Base.repo 到/etc/yum.repos.d/

CentOS 5
    
    wget -O /etc/yum.repos.d/CentOS-Base.repo http://mirrors.aliyun.com/repo/Centos-5.repo
    
CentOS 6
    
    wget -O /etc/yum.repos.d/CentOS-Base.repo http://mirrors.aliyun.com/repo/Centos-6.repo
    
运行yum makecache生成缓存
    
    yum clean all
    yum makecache

# 四、其他repo源 #

    搜狐的Linux安装镜像源：http://mirrors.sohu.com/
    
    北京首都在线科技：http://mirrors.yun-idc.com/
    
