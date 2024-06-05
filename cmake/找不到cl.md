# 找不到 `cl`

Windows 下运行 `cmake` 时报错：

```
The CMAKE_C_COMPILER:

  cl

is not a full path and was not found in the PATH.
```

可以在编译时使用

```shell
cmake -G "MinGW Makefiles"
```

