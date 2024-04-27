# React 项目添加 Tailwind

1. 安装 Tailwind

   ```shell
   npm install tailwindcss postcss-cli autoprefixer
   ```

2. 初始化 Tailwind

    ```shell
    npx tailwindcss init
    ```

    修改 `tailwind.config.js` 文件：

    ```js
    /** @type {import('tailwindcss').Config} */
    module.exports = {
    content: [
        "./src/index.js",
        "./src/**/*.{js,ts,jsx,tsx}",
    ],
    theme: {
        extend: {},
    },
    plugins: [],
    }
    ```

3. 在根目录下创建 `postcss.config.js` 文件：

    ```js
    module.exports = {
    plugins: {
        tailwindcss: {},
        autoprefixer: {},
    },
    }
    ```

4. 修改 `src/index.css` 文件：

    ```css
    @import 'tailwindcss/base';
    @import 'tailwindcss/components';
    @import 'tailwindcss/utilities';
    ```

5. 在 `src/index.js` 文件中引入 `index.css` 文件：

    ```js
    import './index.css';
    ```
