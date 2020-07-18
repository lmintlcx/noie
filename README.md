
# IE 浏览器升级提示

## 预览

<a href="https://www.lmintlcx.com/noie/" target="_blank">点击查看</a>

## 使用

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

## 其他

本项目综合各种因素默认选择了四款浏览器, 并按照现今的市场占有率排名.

- Chrome: Google 出品的最主流的浏览器, 安全快速, 界面简洁, 插件全面.

- Firefox: 开源社区 Mozilla 维护的拥有自己内核的浏览器, 注重隐私保护.

- Edge: Windows 系统自带的浏览器, 使用 Chromium 内核, 方便登录同步.

- Opera: 挪威老牌小众浏览器, 使用 Chromium 内核, 现已被国内收购.

站长在使用时也可以根据自己的需求修改网页内容来自定义所推荐的浏览器, 图像文件夹里已经包含了大部分知名浏览器的图标.

本项目网页被设计成在 IE 浏览器里显示, 推荐列表用像素大小 64x64 的图标基本足够, 如果要兼顾到高分屏以及移动设备, 也可以换成 128x128 192x192 256x256 大小的图标.

~~部分浏览器的官方网站可能已经无法在旧版 IE 浏览器里正常浏览使用了, 站长可以考虑向用户提供所推荐浏览器的离线安装包.~~
