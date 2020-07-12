
# IE 浏览器升级提示

## 预览

[点击查看](https://www.lmintlcx.com/noie/)

## 使用

- 把整个 `noie` 文件夹复制到网站根目录, 使其可以用 `/noie/` 访问到.

- 在需要检测的网页 `<head></head>` 内添加条件跳转.

所有版本:

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
