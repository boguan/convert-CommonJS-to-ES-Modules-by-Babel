## Converting the CommonJS-formatted scripts to ES2015 Modules syntax

### 首先，我们使用 Yarn 安装 babel：

```shell
yarn add --dev @babel/core @babel/preset-env @babel/node
```

### 然后在项目根目录中添加 .babelrc 文件：

```json
{
  "presets": ["@babel/preset-env"]
}
```

### 编辑 index.js

```javascript
import os from 'os';
console.log(os.cpus());
```

### 运行

```shell
yarn babel-node index.js
```

