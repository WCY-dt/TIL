# vmx 版本不兼容

开启虚拟机时报错：

```
*.vmx是由VMware产品创建,但该产品与此版VMware workstation不兼容因此无法使用
```

解决方法如下：

1. 找到虚拟机的 `.vmx` 文件，用文本编辑器打开
2. 修改 `virtualHW.version = "20"` 为正确的版本号
