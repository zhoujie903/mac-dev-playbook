# Mac Development Ansible Playbook

[![Build Status][badge-travis]][link-travis]

[badge-travis]: https://travis-ci.com/zhoujie903/mac-dev-playbook.svg?branch=master
[link-travis]: https://travis-ci.com/zhoujie903/mac-dev-playbook

## 安装

  1. 确定Apple's command line tools 已安装 (`xcode-select --install` 来调走安装)
  2. [安装 Ansible](http://docs.ansible.com/intro_installation.html).
  3. 克隆仓库到本地磁盘
  4. 在目录下运行 `ansible-playbook main.yml -i inventory -K` 

  

> 安装 Ansible
  ```
  $ sudo easy_install pip
  $ sudo pip install ansible
  ``` 

## 测试Playbook
---

* 虚拟机上测试Playbook

* [Travis CI上的持续集成](https://travis-ci.org/zhoujie903/mac-dev-playbook)测试Playbook 


#### 虚拟机安装

在macOS上安装macOS 10.13.6虚拟机可以参考[mac-osx-virtualbox-vm][vm]

首先要有一个`macOS High Sierra.ios`的文件
- `macOS High Sierra.ios`文件可以到网上去查找下载
- 也可以到App Store去下载<https://itunes.apple.com/cn/app/macos-high-sierra/id1246284741?mt=12>，下载完成后文件在`/Applications/Install macOS High Sierra.app`, 然后可以参考[mac-osx-virtualbox-vm][vm]的方法来生成`macOS High Sierra.ios`

自己用`Parallels Desktop Version 13.3.1 (43365)`来安装macOS 10.13.6虚拟机
1. 已下载好`/Applications/Install macOS High Sierra.app`，不需要`macOS High Sierra.ios`文件
2. "File" -> "New"
3. "Install Windows or another OS from a DVD or image file" -> "Continue"![](https://ws3.sinaimg.cn/large/006tNbRwly1fwj9sgfnj3j31g8108qgg.jpg)**注意:** 不要选择底部的`Free Systems`下的`Install macOS 10.14`,好像是在线安装，网速慢费时，且自己安装失败了
4. "Continue"![](https://ws3.sinaimg.cn/large/006tNbRwly1fwj9trxtmej31io12o19a.jpg)
![](https://ws1.sinaimg.cn/large/006tNbRwly1fwj9wi45i6j31io12owvp.jpg) "Continue" -> "Save"会创建一个`/Applications/macOS image file.hdd`的文件
5. "Create" 接下来的安装过程省略

**注意:** 安装成功后，可以删除`/Applications/macOS image file.hdd`文件


[vm]: https://github.com/geerlingguy/mac-osx-virtualbox-vm

---

## Ansible for DevOps

Check out [Ansible for DevOps](https://www.ansiblefordevops.com/), which teaches you how to automate almost anything with Ansible. 

