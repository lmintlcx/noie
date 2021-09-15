
# IE 浏览器升级提示

## 在线预览

<a href="https://www.lmintlcx.com/noie/" target="_blank">点击查看</a>

## 使用方法

1. 把整个 `noie` 文件夹复制到网站根目录, 使其可以用 `/noie/` 访问到.

2. 在需要检测的网页 `<head></head>` 内添加条件跳转.

IE 11 及以下版本和 Edge 旧版:

```html
<script>
  if (/*@cc_on!@*/false || !!document.documentMode || !!window.StyleMedia)
    window.location.href="/noie/";
</script>
```

IE 11 及以下版本:

```html
<script>
  if (/*@cc_on!@*/false || !!document.documentMode)
    window.location.href="/noie/";
</script>
```

IE 10 及以下版本:

```html
<script>
  /*@cc_on window.location.href="/noie/"; @*/
</script>
```

IE 9 及以下版本:

```html
<!--[if lte IE 9]>
  <script>window.location.href="/noie/";</script>
<![endif]-->
```

IE 8 及以下版本:

```html
<!--[if lte IE 8]>
  <script>window.location.href="/noie/";</script>
<![endif]-->
```

IE 7 及以下版本:

```html
<!--[if lte IE 7]>
  <script>window.location.href="/noie/";</script>
<![endif]-->
```

## 默认选择

本项目综合各种因素默认选择了四款浏览器, 并按照现今的市场占有率排名:

- Chrome: Google 出品的最主流的浏览器, 安全快速, 界面简洁, 插件全面.

- Edge: Windows 系统自带的浏览器, 使用 Chromium 内核, 方便登录同步.

- Firefox: 开源社区 Mozilla 维护的拥有自己内核的浏览器, 注重隐私保护.

- Opera: 挪威老牌小众浏览器, 使用 Chromium 内核, 现已被国内企业收购.

> 站长在使用时也可以根据自己的需求修改网页内容来自定义所推荐的浏览器, 图像文件夹里已经包含了绝大部分知名的网页浏览器的图标. 本项目网页被设计成在 IE 浏览器里显示, 因此推荐列表图标用 64x64 的像素大小已经足够, 如果要兼顾到高分屏和移动设备, 也可以换成分辨率为 128x128 192x192 256x256 的图标.

## 项目起源

[旧版 Internet Explorer 淘汰行动](https://support.dmeng.net/kill-old-versions-of-ie.html)
