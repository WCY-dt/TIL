# Github 设置 hosts

1. 从链接中获取hosts：

   - [hosts.gitcdn.top/hosts.txt](https://hosts.gitcdn.top/hosts.txt)
   - [raw.hellogithub.com/hosts](https://raw.hellogithub.com/hosts)

2. 编辑`C:\Windows\System32\drivers\etc\hosts`，加入链接中的hosts

3. 执行

   ```powershell
   ipconfig /flushdns
   ```
