### 创建 TypeScript React 18 项目
npx create-react-app react-ts-app --template typescript

### install package
npm install sass react-router-dom@6 redux react-redux @reduxjs/toolkit

- 安装 Sass（支持 SCSS 样式）
- 安装 React Router v6（路由管理）
- 安装 Redux + Redux Toolkit（状态管理）

### 启动开发服务器
npm start

### 项目结构：
```
react-ts-app/
├─ src/
│  ├─ App.tsx
│  ├─ index.tsx
│  ├─ ...
├─ package.json
├─ tsconfig.json
├─ ...

```

### 在 package.json 里写跨平台方式， 安装 cross-env
npm install --save-dev cross-env

package.json:
```
"scripts": {
  "start": "cross-env PORT=8080 react-scripts start",
  "build": "react-scripts build",
  "test": "react-scripts test",
  "eject": "react-scripts eject"
}
```

