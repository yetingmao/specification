## 前端


#### 环境
##### 1.安装nvm 管理node版本  node 需要两个版本8.16.2和 10+
##### 2.编辑器vscode
##### 3.git
##### 4.yarn（yarn的源设置为淘宝源）


### 前端开发

#### 变量
######  使用驼峰命名
######  使用let(不许使用var)


#### 常量
###### 使用全部字母大写，单词间下划线分隔的命名方式。
###### 使用const(不许使用var)


####  判断 True 和 False 
###### 优先使用 typeof
###### 值为boolean可直接判断，其他类型判断是否undefined  |  null 
###### 使用 ===


####  文件命名 
###### 默认为index.js/ts/html 
###### style.css/less/sass 


####  导入命名 
###### export default 导出时，导入的名字首字符大写
###### export XXX ，导入名字一样 


####  字符串拼接 
###### 使用字符串模板


#### 开发流程（gitlab）
##### 仓库：源仓库（线上），开发者仓库（本地）
##### 分支
###### master：主分支， 经过测试，已经完全稳定的代码，可以当做产品供用户使用的代码。要随时保持master分支代码的清洁与稳定。
###### develop：开发分支，开始是从master切换出来，用于开发者存放基本稳定的代码。
###### feature：功能分支，用于开发者开发项目功能的分支，一般从本地develop分支切出来，在该分支上开发。

``` 
    //开发新功能，在gitlab源仓库创建一个分支some-feature，基于源仓库develop

    //本地
    git checkout  develop //切换到develop分支

    git checkout -b some-feature //分出一个功能性分支

    touch XXX.js //开发

    git add . 
    git commit -m "增加什么什么功能"  //测试之后存到本地仓库

    git pull origin some-feature
    git push origin some-feature  // 提交到源仓库的功能分支

    //在gitlab上  some-feature  pull request  develop
    
    //管理员对功能分支review,没有问题就merge到develop分支
    
```

#### 代码格式
###### vscode插件 
###### 在vscode配置
###### setting->setting.json
###### 保存时会自动格式化代码
```
    "editor.formatOnType": true,
    "editor.formatOnPaste": true,
    "editor.formatOnSave": true,
    
```
#### 推荐vscode插件
######  koroFileHeader（在vscode中用于生成文件头部注释和函数注释的插件）
###### 头部window：ctrl+alt+i,mac：ctrl+cmd+i
###### 光标处window：ctrl+alt+t,mac：ctrl+cmd+t （可能会有快捷键冲突，网上搜索可解决）
###### 在vscode配置
```
 "fileheader.customMade": { //此为头部注释
        "Description": "",
        "Autor": "yetm", //作者
        "Date": "Do not edit",
        "LastEditors": "yetm",
        "LastEditTime": "Do not edit"
    },
    "fileheader.cursorMode": { //此为函数注释
        "description": "",
        "param": "",
        "return": "", 
        "author": "yetm" //作者
    }
```

###### Bracket Pair Colorizer（在vscode中用于以括号颜色来辨识开始结束内容的插件）
###### Auto Close Tag 自动关闭标签
###### Auto Complete Tag 自动完成补齐标签  
###### Auto Import 自动导入 
###### Auto Rename Tag 自动改正标签 GitLens — Git supercharged
###### GitLens — Git supercharged  git记录 
###### JavaScript (ES6) code snippets js语法提示
###### npm Intellisense require包时会提示 
###### Path Autocomplete 路径自动补充
###### Path Intellisense 路径提示
###### Sass/Less/Scss/Typescript/Javascript/Jade/Pug Compile Hero Pro 写css时提示
###### Vetur 写vue提示 
###### vscode-icons 文件管理的树目录显示图标

 
--- 

## 前端第三方包

##### vue拖拽插件   <a href="https://www.npmjs.com/package/vuedraggable">vuedraggable</a>

##### vue文字无线滚动   <a href="https://github.com/chenxuan0000/vue-seamless-scroll">vue-seamless-scroll</a>

##### 静态资源管理，局域网内的可以访问 （简单方便） <a herf="https://github.com/JacksonTian/anywhere">anywhere </a>

##### JavaScript 实用工具库  <a href="https://www.lodashjs.com/">lodash</a>

##### JavaScript 一个超轻量级的时间处理工具库  <a href="https://www.npmjs.com/package/dateformat">dateformat.js</a>

###### 后续再添加...

## 推荐工具

##### 命令行工具   gitBash/<a href="https://cmder.net/">cmder</a> 建议full版本 （cmder是一个增强型命令行工具，不仅可以使用windows下的所有命令，还可以使用linux的命令,shell命令。）
##### 可以集成到vscode
###### setting->setting.json

```
    //git
    "terminal.integrated.shell.windows": "C:\\Program Files\\Git\\bin\\sh.exe",  //安装路径

    //cmder
    "terminal.integrated.shell.windows": "C:\\Windows\\System32\\cmd.exe",
    "terminal.integrated.shellArgs.windows": [
        "/K",
        "D:\\Program Files (x86)\\cmder\\vendor\\init.bat"    //安装路径执行bat的文件
    ],
```


--- 


## 前端技术栈


##### 前端框架 vue/react

##### 前端ssr框架 nuxt.js(vue)/next.js(react)/umi.js(react)

##### 前端UI框架 elementUI(vue)/iview(vue)/ant-design-vue(vue)/Ant Design(react)/Material-UI(react)

##### 前端测试框架 jest

##### 前端可视化图形 echarts/antv

##### 前端状态管理  dva/mbox/redux

##### javascript类型管理  typescript


---
## 后续再添加