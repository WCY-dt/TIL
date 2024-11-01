# Matplotlib 绘制中文

1. 安装 `mplfonts`

    ```shell
    pip install mplfonts
    ```

2. 初始化 `mplfonts`

    ```shell
    mplfonts init
    ```

3. 使用中文

    ```python
    import matplotlib.pyplot as plt
    from mplfonts import use_font
    use_font("SimHei")
    ```
