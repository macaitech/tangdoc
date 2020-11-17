### 1.列表

用途|使用|案例
-|-|-
无序列表|使用 *，+，-|表示无序列表 
有序列表|需用序号|1. 有序列表项 一
缩进列表|使用 *|-
引用列表|使用>|
代码块|使用2个tab|


*	神奇的网站

    > 打开书本。
    > 打开电灯。


### 2.代码块
代码块,使用2个tab,或使用六个\`

		yum -y install epel-release
		yum -y install socat

行内式，使用两个\`包裹起来

C语言里的函数 `scanf()` 怎么使用？
### 3. 斜体和粗体

		*斜体*或_斜体_
		**粗体**
		***加粗斜体***
		~~删除线~~

### 4.超链接

#### a.行内式
	
		欢迎来到[百度](http://www.baidu.com)
		
#### b.参考式

		我经常去的几个网站[GitHub][1]、[知乎][2]
		
		[1]:https://github.com "GitHub"
		[2]:https://www.zhihu.com "知乎"	

我经常去的几个网站[GitHub][1]、[知乎][2]

[1]:https://github.com "GitHub"
[2]:https://www.zhihu.com "知乎"

### c.自动链接

		<http://example.com/>
		<address@example.com>
		
### 5.锚点
何添?加页面内锚点
		
		跳转到[目录](#autolink)


### 6.特殊字符

行首出现数字-句点-空白,在句点前面加上反斜杠

1986. What a great season.		
1986\. What a great season. (在句点前面加上反斜杠)


### 7.引用

#### a.单层引用

引用需要在被引用的文本前加上>符号

		> 这是一个有两段文字的引用,
		>无意义的占行文字1.

> 这是一个有两段文字的引用,
>无意义的占行文字1.
>无意义的占行文字2.
>
>无意义的占行文字3.
>无意义的占行文字4.


#### b.多层引用

区块引用可以嵌套（例如：引用内的引用），只要根据层次加上不同数量的 >：

		>>> 请问 Markdwon 怎么用？ - 小白
		>>自己看教程！ - 愤青
		>教程在哪？ - 小白

>>> 请问 Markdwon 怎么用？ - 小白

>>自己看教程！ - 愤青

>教程在哪？ - 小白


### 8.插入图片

#### a.行内式

语法说明： 

		![图片Alt](图片地址 "图片Title")

![快乐学习](https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=1271887439,937829543&fm=26&gp=0.jpg "快乐学习")


#### b.参考式

语法说明： 

		在文档要插入图片的地方写![图片Alt][标记]
		在文档的最后写上[标记]:图片地址 "Title"

		梵高：
		![梵高][fangao]
		
		[fangao]:http://upload-images.jianshu.io/upload_images/10016597535c9e3fe16240d?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240 "梵高"

		

### 9.注脚


使用 Markdown[^1]可以效率的书写文档, 直接转换成 HTML[^2], 你可以使用简书或者支持Markdown的编辑器进行书写。

[^1]:Markdown是一种纯文本标记语言

[^2]:HyperText Markup Language 超文本标记语言


### 10.数学公式

```tex
   E=mc^2
```


### 11.分隔线

		使用***，独立成行，就是分割线
		
***

### 12.原始HTML

```
<table>
    <tr>
        <th rowspan="2">值班人员</th>
        <th>星期一</th>
        <th>星期二</th>
        <th>星期三</th>
    </tr>
    <tr>
        <td>李强</td>
        <td>张明</td>
        <td>王平</td>
    </tr>
</table>
```
效果:

<table>
    <tr>
        <th rowspan="2">值班人员</th>
        <th>星期一</th>
        <th>星期二</th>
        <th>星期三</th>
    </tr>
    <tr>
        <td>李强</td>
        <td>张明</td>
        <td>王平</td>
    </tr>
</table>


### 13.todo list

```
近期任务安排:
- [x] 整理Markdown手册
- [ ] 改善项目
   - [x] 优化首页显示方式
   - [x] 修复闪退问题
   - [ ] 修复视频卡顿
- [ ] A3项目修复
   - [x] 修复数值错误
```

近期任务安排:
- [x] 整理Markdown手册
- [ ] 改善项目
   - [x] 优化首页显示方式
   - [x] 修复闪退问题
   - [ ] 修复视频卡顿
- [ ] A3项目修复
   - [x] 修复数值错误
   
   
 ### 14.注释
 
```
	使用 [comment]:或[//]:将本行内容注释
```

[comment]: 使用将本行内容注释
