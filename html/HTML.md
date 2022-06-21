# HTML

## 1.meta的用法和结构

`<meta>`元素用于表示网页的元素就

```html
<head>
  <meta charset="" http-equiv="" name="" content=""/>
</head>
```

`charset`  这个属性声明了文档的字符编码。如果使用了这个属性，其值必须是与 ASCII 大小写无关（ASCII case-insensitive）的"`utf-8`"。

`http-equiv`  定义一个编译指示指令,所有允许的值都是特定 HTTP 头部的名称，如下：

- `content-security-policy`  内容策略主要指定允许的服务器源和脚本端点，这有助于防止跨站点脚本攻击。
- `content-type`  如果使用这个属性，其值必须是"`text/html; charset=utf-8`"。注意：该属性只能用于 [MIME type](https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Basics_of_HTTP/MIME_types) 为 `text/html` 的文档，不能用于 MIME 类型为 XML 的文档。
- `default-style`   设置默认 [CSS 样式表](https://developer.mozilla.org/zh-CN/docs/Web/CSS)组的名称。
- `x-ua-compatible`  如果指定，则 `content` 属性必须具有值 "`IE=edge`"。用户代理必须忽略此指示。
- `refresh`   这个属性指定：
- 这个属性指定：
  - 如果 [`content`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/meta#attr-content) 只包含一个正整数，则为重新载入页面的时间间隔 (秒)；
  - 如果 [`content`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/meta#attr-content) 包含一个正整数，并且后面跟着字符串 '`;url=`' 和一个合法的 URL，则是重定向到指定链接的时间间隔 (秒)
- `name`   `name` 和 `content` 属性可以一起使用，以名 - 值对的方式给文档提供元数据，其中 name 作为元数据的名称，content 作为元数据的值。



## 2. HTML5 标记

### 2.1 文本标签

```html
<pre></pre> 标记保留文本所有换行与空格
<hr></hr> 水平线
<cite></cite> 用于定义作品的标题，表现为斜体形式
<ins></ins> 表示插入的文本
<dle></dle> 表示删除的文本
<sub></sub>下标文本
<sup></sup> 上标文本
```



### 2.2 列表 

```html
<ul>
    <li>无序列表</li>
</ul>
<ol>
    <li>有序列表</li>
</ol>
<dl>
    <dt>描述列表</dt>
    <dd></dd>
</dl>
```

## 3. 媒体

### 3.1 图片标签

```hmtl
<img src="" alt="" height="" width="" />
```



### 3.2 视频标签

```html
<video src=" " controls="controls" autoplay="autoplay" width=" " height="" preload=" " loop="loop">您的浏览器不支持video(当浏览器不支持video时显示)</video>
<!--这是视频的标准语法,标签中的文字是当视频加载不成功的时候才会显示出来的-->
<!--
	controls="controls"添加浏览器为视频设置的默认控件 
	autoplay="autoplay"设置网页中视频加载就绪后自动播放 
	loop="loop"设置媒介文件循坏播放
	preload="auto/none/meta" 值:1.none表示不加载任何视频 2.meta表示只加载元数据（长度，尺寸等 3.auto表示让浏览器自己决定怎么做（如果引用了autoplay属性，则忽略该属性）
	poster='' ‘’指定加载视频时要显示的图像，接受所需图像的URL(如果引用了autoplay属性，则忽略该属性)	使用方法：<video poster="网址"></video>
	muted="muted" 设置是否静音
-->
```





