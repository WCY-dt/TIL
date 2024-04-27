# React 项目添加 TypeScript

1. 安装 TypeScript

   ```shell
   npm install typescript @types/node @types/react @types/react-dom
   ```

2. 初始化 TypeScript

   ```shell
    npx tsc --init
    ```

    修改 `tsconfig.json` 文件：

    ```json
    {
        "compilerOptions": {
            "jsx": "react",
            "target": "es2020",
            "module": "commonjs",
            "esModuleInterop": true,
            "forceConsistentCasingInFileNames": true,
            "strict": true,
            "noImplicitAny": true,
            "noImplicitOverride": true,
            "noImplicitReturns": true,
            "skipLibCheck": true
        }
    }
    ```

3. 除了 `index.js` 外，将所有 `.js` 文件改为 `.tsx` 文件。如果文件中没有 JSX 语法，也可以将后缀改为 `.ts`
