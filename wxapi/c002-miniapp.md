[//]:微信小程序


### 一、小程序基本介绍

- 相对于H5，小程序提供了贴近原生APP的体验。相对于原生APP，小程序提供了快速开发的能力。
- 要进行小程序开发，首先要有开发者账号，申请开发小程序，并下载小程序开发工具：[小程序开发工具](https://developers.weixin.qq.com/miniprogram/dev/devtools/download.html)
- 通过 sitemap.json 配置，运行微信搜索爬虫收录小程序。
- 小程序框架的逻辑层并非运行在浏览器中，因此 JavaScript 在 web 中一些能力都无法使用，如 window，document 等。
- 整个小程序只有一个 App 实例，是全部页面共享的。开发者可以通过 getApp 方法获取到全局唯一的 App 实例。
- 模块化，可以将一些公共的代码抽离成为一个单独的 js 文件，作为一个模块。模块只有通过 module.exports 或者 exports 才能对外暴露接口。

#### 二、小程序目录与宿主环境


##### 1、目录配置
- a、.json 后缀的 JSON 配置文件  

文件|用途
-|-
app.json|小程序全局配置,包括了小程序的所有页面路径、界面表现、网络超时时间、底部 tab 等。
project.config.json|开发工具配置 
page.json|页面配置，小程序里边的每个页面都可以配置自己的页面风格
pages/logs/logs.json|

- b、.wxml 后缀的 WXML 模板文件  
- c、.wxss 后缀的 WXSS 样式文件  
- d、.js 后缀的 JS 脚本逻辑文件  
- e、其他介绍

文件|用途
-|-
app.js|小程序逻辑。
app.json|小程序公共配置
app.wxss|小程序公共样式表

js：页面逻辑 ,wxml：页面结构json：页面配置 ,wxss：页面样式表。描述页面的四个文件必须具有相同的路径与文件名 ,

##### 2、运行环境
整个小程序框架系统分为两部分：逻辑层（App Service）和 视图层（View）。小程序提供了自己的视图层描述语言 WXML 和 WXSS，以及基于 JavaScript 的逻辑层框架，并在视图层与逻辑层间提供了数据传输和事件系统，让开发者能够专注于数据与逻辑。其中 WXML 模板和 WXSS 样式工作在渲染层，JS 脚本工作在逻辑层。  
 <img src="https://res.wx.qq.com/wxdoc/dist/assets/img/4-1.ad156d1c.png" height = "500" alt="小程序的运行环境" align=center />
 
 #### 三、小程序开发
 
 ##### 1、小程序视图层
 
- 框架的视图层由 WXML 与 WXSS 编写，由组件来进行展示。

- 将逻辑层的数据反映成视图，同时将视图层的事件发送给逻辑层。

- WXML(WeiXin Markup language) 用于描述页面的结构，页面标签语言。

- WXS(WeiXin Script) 是小程序的一套脚本语言，结合 WXML，可以构建出页面的结构。

- WXSS(WeiXin Style Sheet) 是一套样式语言，用于描述 WXML 的组件样式。

- 组件(Component)是视图的基本组成单元。

 ##### 2、组件
 
 - 事件是视图层到逻辑层的通讯方式。
- 事件可以将用户的行为反馈到逻辑层进行处理。
- 事件可以绑定在组件上，当达到触发事件，就会执行逻辑层中对应的事件处理函数。
- 事件对象可以携带额外信息，如 id, dataset, touches。
 
