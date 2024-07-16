# WSL 配置 ssh 连接 GitHub

1. 生成 ssh key

  ```bash
  ssh-keygen
  ```

2. 查看生成的 ssh key

  ```bash
  cat ~/.ssh/id_rsa.pub
  ```

  并将其添加到 GitHub 的 [SSH and GPG keys](https://github.com/settings/keys) 中

3. 将 ssh key 添加到 ssh-agent 中

  ```bash
  eval $(ssh-agent -s)
  ssh-add ~/.ssh/id_rsa
  ```

4. 连接 GitHub 测试

  ```bash
  ssh -T git@github.com
  ```
