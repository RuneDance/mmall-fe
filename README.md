
##项目初始化步骤

* 安装nodejs环境,推荐使用v6.12.3
    下载地址 : https://nodejs.org/download/release/v6.12.3/

* 在项目根目录执行npm初始化
    命令: npm install --registry=https://registry.npm.taobao.org

* 启动项目
    开发模式: npm run dev (windows系统上为npm run dev_win)
    生产模式: npm run dist (windows系统上为npm run dist_win)

* 开发模式下预览项目
    访问：http://localhost:8088/dist/view/index.html


---
##mmall-fe v1.0.1改动：

* 升级nodejs版本到6.12.3（升级后需要把原项目中node_modules目录删除，重新执行初始化）

* hogan插件被废弃，替换为hogan.js

* 启动方式改动，不再需要安装全局的webpack和webpack-dev-server（需要nodejs版本在6.12.3）

* 移除webpack-dev-server里的client注入，webpack-dev-server可以自动注入client了

* 添加devServer的proxy选项，开发模式下可以直接访问接口，不再需要charles或fiddler做代理

* 将启动命令中的inline和port选项从命令移到了配置文件中

## 环境搭建
```
1、npm install webpack -g 全局安装 (windows系统全局不要安装最新的webpack默认和局部安装的版本保持一致)(npm uninstall webpack -g)
2、npm init
3、npm install webpack@4.2.0 --save-dev

充:npm install --save-dev webpack-cli    (2.0.13)

4、webpack -v 查看版本号
 全局安装 不用版本号 局部安装 需要版本号
 
 5、npm install jquery --save
 6、npm uninstall jquery --save
 
 7、npm install css-loader style-loader --save-dev
 8、npm install extract-text-webpack-plugin@4.0.0-beta.0 --save-dev
 9、npm install html-webpack-plugin --save-dev
 10、npm install html-loader --save-dev
 11、npm install url-loader --save-dev
 12、npm install webpack-dev-server@3.1.1 --save-dev (npm install webpack-dev-server@3.1.1 -g)
充:  npm install file-loader@1.1.11 --save-dev
 13、npm install font-awesome@4.7.0 --save
 14、npm install hogan.js --save
```