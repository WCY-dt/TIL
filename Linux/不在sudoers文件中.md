# 不在 sudoers 文件中

使用 `sudo` 命令时，提示 `xxx 不在 sudoers 文件中。此事将被报告。`，这是因为当前用户没有权限使用 `sudo` 命令。

首先切换到 `root` 用户：

```bash
su
```

然后编辑 `/etc/sudoers` 文件：

```bash
sudo nano /etc/sudoers
```

找到 `%sudo ALL=(ALL:ALL) ALL` 这一行，在下方添加一行：

```bash
用户名 ALL=(ALL:ALL) ALL
```

保存退出，回到之前的用户即可。
