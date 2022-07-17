# Linux基础
    cpu架构：
        x86
        x64(amd64)
        m68000-->m68k
        arm
        ultrasparc：solaris
        power：AIX
        powerpc-->ppc
        MIPS
        alpha：hp-ux
        ...
        每种cpu->机器语言->汇编语言->高级语言
    移植：portable
        编译器将高级语言源码翻译为指定架构汇编语言
    cross compile
        hardware specific->kernel->sys call->lib
    POSIX:lib 标准化接口
        API：application program interface
        ABI：application binary interface
    linux，bsd，aix...:unix-like 
        unix类的系统：兼容
            API
            ABI
# 程序管理
    程序的组成：
        二进制程序
        配置文件
        库文件
        帮助文件
    程序包管理器：
        程序的组成文件打包成一个或有限几个文件
        安装：展开包文件到指定位置
        卸载：根据安装配置，删除对应文件
        查询：确认版本，路径等信息
        debian：dpkg，apt-get
        redhat：rpm，yum，dnf
        archlinux：pacman
        Suse：rpm，zypper
        