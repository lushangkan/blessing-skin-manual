# 皮肤站 CDN 配置

在「资源配置」页面使用「前端资源文件 CDN」，并使用自建或他人搭建好的 CDN 服务，皮肤站所有的静态文件（CSS/JS）都会从 CDN 请求，可减轻源站的负担。

## 如何自建皮肤站 CDN？

将皮肤站（必须是编译后的，直接从 GitHub 上下的源码不行） `/public` 目录下的文件全部复制到你的 CDN 服务器的某个你喜欢的地方，并保证它们能被外界访问到。

按照你的具体情况，填写「前端资源文件 CDN」。如果你把资源文件放在 CDN 服务器上的某个子目录中的话，「CDN 地址」里也要带上那个子目录。

不知道怎么填写才对？访问 `{你应该填写的地址}/app/manifest.json`，如果正常显示，那就可以了。

## 目前可用的公共 CDN

由第三方维护，选择其中一个地址填入「静态文件 CDN」插件配置页面中即可。

::: danger 小心！
注意，我们无法 100% 保证第三方 CDN 的安全。请谨慎使用，防止恶意代码的注入。
:::

|名称|地址|
|-|-|
|hempflower|https://bs-mirror.i-creator.cn/v4/|

::: tip 想要提交新的公共 CDN？
请在 [bs-community/blessing-skin-manual](https://github.com/bs-community/blessing-skin-manual) 下提一个 Issue 或直接发起 Pull Request。
:::
