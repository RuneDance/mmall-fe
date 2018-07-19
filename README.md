## 项目初始化步骤
```
安装nodejs(v6.12.3)环境
    下载地址 : https://nodejs.org/download/release/v6.12.3/
在项目根目录执行npm初始化
    命令: npm install --registry=https://registry.npm.taobao.org
全局安装
    npm install xxxxx -g    (npm uninstall xxxxx -g)
局部安装
    npm install xxxxx --save-dev (npm uninstall xxxxx --save-dev)
    npm install xxxxx --save (npm install xxxxx --save)
安装步骤：
    1、npm install webpack -g  
    2、npm init
    3、npm install webpack@4.2.0 --save-dev 安装webpack
    4、webpack -v 查看版本号
    5、npm install css-loader@0.28.11 extract-text-webpack-plugin@4.0.0-beta.0 file-loader@1.1.11 font-awesome@4.7.0 html-loader@0.5.5 html-webpack-plugin@3.2.0 style-loader@0.21.0 url-loader@1.0.1 webpack-cli@2.1.4 webpack-dev-server@3.1.1 --save-dev
    6、npm install font-awesome@4.7.0 hogan.js@3.0.2 --save
启动项目：
    开发模式: npm run dev (windows命令为：npm run dev_win)
    生产模式: npm run dist (windows命令为：npm run dist_win)
开发模式下访问：
    http://localhost:8088/dist/view/index.html
```

## mmall-fe(v1.0.1) 说明：
```
升级nodejs版本到6.12.3（升级后需要把原项目中node_modules目录删除，重新执行初始化）

hogan插件被废弃，替换为hogan.js

启动方式改动，不再需要安装全局的webpack和webpack-dev-server（需要nodejs版本在6.12.3）

移除webpack-dev-server里的client注入，webpack-dev-server可以自动注入client了

添加devServer的proxy选项，开发模式下可以直接访问接口，不再需要charles或fiddler做代理

将启动命令中的inline和port选项从命令移到了配置文件中
```