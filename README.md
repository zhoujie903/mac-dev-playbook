# Mac Development Ansible Playbook

[![Build Status][badge-travis]][link-travis]

[badge-travis]: https://travis-ci.com/zhoujie903/mac-dev-playbook.svg?branch=master
[link-travis]: https://travis-ci.com/zhoujie903/mac-dev-playbook

## 安装

  1. Ensure Apple's command line tools are installed (`xcode-select --install` to launch the installer).
  2. [安装 Ansible](http://docs.ansible.com/intro_installation.html).
  3. 克隆仓库到本地磁盘
  4. 在目录下运行 `ansible-playbook main.yml -i inventory -K` 

## 测试Playbook

在虚拟机上测试Playbook

也可以在[Travis CI上的持续集成](https://travis-ci.org/zhoujie903/mac-dev-playbook)测试Playbook

关于macOS 10.13.6虚拟机安装可以参考<https://github.com/geerlingguy/mac-osx-virtualbox-vm>

首先要有一个`macOS High Sierra.ios`的文件
- `macOS High Sierra.ios`文件可以到网上去查找下载
- 也可以到App Store去下载<https://itunes.apple.com/cn/app/macos-high-sierra/id1246284741?mt=12>，下载完成后文件在`/Applications/Install macOS High Sierra`, 然后可以参考<https://github.com/geerlingguy/mac-osx-virtualbox-vm>的方法来生成`macOS High Sierra.ios`

## Ansible for DevOps

Check out [Ansible for DevOps](https://www.ansiblefordevops.com/), which teaches you how to automate almost anything with Ansible. 

