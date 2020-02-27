# Actions-pve-kernel

Linux Kernel for Proxmox projects

Build Proxmox VE Kernel for J3455 with IOMMU using GitHub Actions

根据koolshare 上 emile239 提出解决Proxmox VE 6.x下J3455主板直通iommu分组问题的方法编译Proxmox Kernel。

自动从git://git.proxmox.com/git/pve-kernel.git 拉取master分支代码，并自动修改patch文件，让内核使用特制的ACS_override补丁。

# 注意事项
最新代码生成的文件中 linux-tools-5.3-dbgsym 文件为ddeb格式，所以需要注意调整相应的安装dpkg命令。
