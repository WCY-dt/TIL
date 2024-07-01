# VMware Tools 无法直接安装

在 VMware Workstation 中，虚拟机的 `虚拟机` 菜单中有一个 `安装 VMware Tools` 选项，但是在某些情况下，这个选项是灰色的，无法点击。这时可以尝试以下方法：

1. 关闭虚拟机
2. 进入虚拟机的设置页面，找到 `CD/DVD (SATA)`
3. 选择 `使用 ISO 镜像文件`，然后选择 `C:\Program Files (x86)\VMware\VMware Workstation\linux.iso`（路径可能不同）
4. 重新启动虚拟机，然后再次尝试安装 VMware Tools
