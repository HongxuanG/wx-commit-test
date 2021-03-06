# wechat_applet_demo

> 如无意外不会更新了，请移步至 [cosscomb-mini](https://github.com/toFrankie/csscomb-mini)。

利用 ESLint、Prettier、git hooks 等工具“一键偷懒”，哈哈。😆

本项目说明放在[简书](https://www.jianshu.com/u/f4dac74bd955)更新：

* [使Prettier一键格式化WXSS（上集）](https://www.jianshu.com/p/5ab7b4b48964)
* [使Prettier一键格式化WXSS（下集）](https://www.jianshu.com/p/0f7ba22d18cd)
* [使Prettier一键格式化WXSS（结局篇）](https://www.jianshu.com/p/553cef04e262)

说明一下：在 `tags-v1.0.0` 👉 [wechat_applet_demo-1.0.0](https://github.com/toFrankie/wechat_applet_demo/releases/tag/v1.0.0) 是利用了 Gulp.js，而最新方式已经移除 Gulp 及其相关依赖包。

<hr/>

### 为什么要做这件事情？

原因是这样的，原本在 H5 项目中，使用 ESLint、Prettier 是水到渠成的，但是放到小程序项目中去的时候，总有一些事不顺心的，比如 Prettier 无法识别微信小程序的 `.wxss`、支付宝小程序的 `.acss` 层叠样式，那么之前愉快的一键操作就不能继续玩耍了。

让 Prettier 也识别小程序的层叠样式文件，有两种解决方式：

* 使用 Gulp.js（它利用了 Node.js 的流）来进行格式的转换，先转换成可被 Prettier 识别的文件（如 CSS），再将其转换回原来的文件。（已弃用）
* 利用 Prettier 提供的 Overrides、Parser 选项，指定使用对应的解析器。


### 为什么喜欢在简书上写文章？

1. 多端支持，无用手机、iPad、电脑、网页我都能看到最新的文章，同步效果很好。
2. 最主要是看上了它的 Markdown 编辑，太好用了
3. 不在掘金更新，是因为自己还不够格，扛不住大佬们的评论啊，哈哈。我想总会有一天的...

### 为什么要写文章？

我看过一个 Q&A，大致的意思是：

Q：网上充斥着各种文章，比你写的要好的比比皆是，你为什么还要再写一遍。

A：那些文章即使让你看见了，但可能还不是你的...

我非常认同这个观点，因为我在写文章的过程中，可以查漏补缺，可以看到一些平时一闪而过被忽略的知识点，最重要是能加深印象和理解。

哪天我可能会忘掉，但我回来看一下，当初写文章那种思路似乎瞬间就回来了，因为它就是按照你的思路去写出来的文章啊。

🎉 牛批吹完了，继续搬砖...