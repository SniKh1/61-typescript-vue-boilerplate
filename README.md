# A nice `typescript+vue` development framework by 61
  - support  mutilple entry mode
## Install
```
git clone https://github.com/SniKh1/61-typescript-vue-boilerplate.git
// or use iclone-cli
// first install `iclone-cli` in global
npm i -g iclone-cli
// then
iclone init -t ts-vue -n [projectName]
```

## Startup

### run in dev mode

> npm start

### build in production

> npm run build:prod

### Catalog

```
├── README.md
├── build
├── dev-config
|  ├── configs
|  ├── index.template.html
|  ├── lite-server-config.js
|  ├── readme.md
|  └── webpack.config.js
├── dist
├── docs
|  └── README.md
├── package.json
├── src
|  ├── assets
|  ├── common
|  ├── components
|  ├── apps
|  ├── globals.d.ts
|  ├── index.ts
|  ├── routes
|  └── utils
├── tsconfig.json
├── tslint.json
└── yarn.lock
```

### `vue` develop help
1. 在less中使用import如果想使用别名路径可以使用~开头：
```
//style.less
@import '~@/common/main.less'
```
### Updates
1. add `tslint` task
2. add `tslint-loader`
  - 会自动格式化错误的代码风格
3. add `stylelint-loader`
  - 会自动格式化错误的代码风格
4. add了自定义模板
  - 只需要在 `./src/apps/` add与 `xxx.ts` 同文件名的 .html文件则自动采用此模板
  - 比如: `./src/apps/xx.ts` 对应  `./src/apps/xx.html`
  - 如果文件名以 `_`开头则忽略掉对应的文件
5. add css modules
6. `webpack-dev-server` 添加 `host: '0.0.0.0'` 配置局域网内可访问
