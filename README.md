# 实验指南

由于Openeuler的网上参考资料很少，而且很多人应该对命令行不熟练，配置相对困难，写下该指南，请大佬斧正

## 实验环境

- Openeuler
- vscode

## 实验一

- 配置环境



1. 下载iso文件

   - 可以从openeuler官网或者[清华镜像下载](https://mirrors.tuna.tsinghua.edu.cn/openeuler/openEuler-20.03-LTS/ISO/) 

2. 安装vmware

3. 安装虚拟机

   - 理论上配置越高越好
   - 系统的安装有图形化界面，按照指示就没有什么困难

4. 配置源

   - openeuler没有预置源也没有图形界面，既没有vim也没有nano，只能使用vi

   - 在文件中加入以下内容，若依然无法使用``` sudo dnf install``` 则将gpgcheck修改为0

     ```
     # /etc/yum.repos.d/openEuler_x86_64.repo
     [osrepo]
     name=osrepo
     baseurl=https://repo.openeuler.org/openEuler-20.03-LTS/OS/x86_64/
     enabled=1
     gpgcheck=1
     gpgkey=https://repo.openeuler.org/openEuler-20.03-LTS/OS/x86_64/RPM-GPG-KEY-openEuler
     ```

5. 桌面

   - 个人未配置桌面
   - 如果实在无法忍受命令行，可以安装gnome桌面 [传送门](https://zhuanlan.zhihu.com/p/229861153) 

6. 远程编辑

   - 可以使用xshell远程登录编辑
   - 