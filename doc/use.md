# jekyll_theme
[简体中文](/use.md) | Sorry, We do not have English instructions for use now.
## 欢迎
欢迎你的到来，你一定非常想使用这个项目吧。<br>那请您一定仔细阅读下面的使用说明。

---

## 使用
> 注：因为我们是基于[Kotet的项目](https://github.com/kotet/ultralight)制作的，Kotet并没有制作详细的使用教程，如果Kotet更新了使用教程，一定要去看哦~！
### 下载与更新
请在我们的Release界面或去往此项目的官网下载此主题的压缩包(zip文件)。

Release界面链接：
- [Github](https://github.com/ZiChenStudio/Efficiency_jekyll_theme/releases)
- [Gitee](https://gitee.com/ZiChenStudio/Efficiency_jekyll_theme/releases)

> Tips:请选择对你来说方便的下载源。<br>更新请自行检查Release界面<br>一般情况下，Github的Release更新更快！

此项目的官网：
- [HERE](https://efficiencytheme.netlify.app/)

> Tips:强烈建议使用官网下载，因为里面有更加详细的解释说明。<br>一般情况下，官网的更新速度比Github的Release更新更快。
#### 下载的版本选择
去往官网可以看到具体的版本解释

版本号为：x.x.x的为非Mini版;<br>
版本号为：x.x.x.x的为Mini版;<br>
非Mini版的版本需要自行去官网查看版本。

### 模版
在你下载的压缩包，或我们的储存库的src文件夹中的两个文件夹中存放我们的模版。分别是：
```
_include
_layout
```
其中_include文件夹中的footer.md是页脚文件，可以进行更改；<br>head.html是网页头部文件，可进行更改。

_layout文件夹存放的default.html是默认模版，所有的html文件生成都要经过它<br>home.html是主页文件，只要主页经过它生成；<br>post.html是文章的模版，可以更改；

其他的文件最好不要进行更改，如果您更改了其中您不了解的内容，项目可能会发生错误甚至无法工作。
###  文章
在你下载的压缩包，或我们的储存库的src文件夹中的一个文件夹中存放着文章文件夹。是：
```
_posts
```
这里的文件要符合规则命名，规则如下：
```
yyyy-mm-dd-name.md
```
也就是说年份要四位数，例如：
```
1900
```
月份要二位数，例如：
```
09
```
日期要二位数，例如：
```
01
```
中间用英文减号隔开，也就是：
```
-
```
name处写你的文件名，这跟你的文章标题没有关系，最好用英文的

正确命名举例：
```
2022-09-01-welcome.md
```
注意，文件的后缀是 md ，并不是 html 。
### 运行
如果你要生成html文件，请在根目录下运行命令：
```
jekyll server
```
出现done in xxx seconds.之后停止运行

你的html文件就生成在_site文件夹下了
### 文章
所有你想生成的文章都要放置在 _posts 文件夹中。

在你想生成的文件的最顶部写头信息：
```
---
layout: post
title: name
tags: tag
---
```
其中 name 处写你的文章的标题，tag 处写你的文章的标签，如果你想让你的文章同时拥有两个标签，请在这两个标签中添加一个英文状态下的空格。

正确头信息例子：
```
layout: post
title: 第一个文章
tags: test
```
### 超链接
如果你想添加其他文章的超链接请在文章.md中输入：
```
[NAME](./../../yyyy/mm/dd/name.md)
```
例子：
```
如果文章的文件名是 2022-09-01-welcome.md
那超链接的名字就是
[超链接名字](./../../2022/09/01/welcome.md)
```
#### 为什么不使用{% link _posts/yyyy-mm-dd-name.md %}
因为网站目录的问题，我们使用时通常把它放在文件夹里，而不是根目录。

```
{% link _posts/yyyy-mm-dd-name.md %}
```
这种方式会直接定位到根目录，有点问题。
### 引导
在我们的项目的src文件夹中的 index.md 是引导文件，里面可以编辑标题等信息(我们这边只建议改标题)

about.md 是About界面的消息，可以自行添加内容，例如联系方式等内容，方便他人找到你。

tags.md 是Tag标签的页面，可以更改里面的标题。(我们这边只建议改标题，并不建议您在没有搞懂源代码的情况下进行更改)

404.html 放置的是网页的404界面，可以自行更改。
### 图标
网站的图标放置在 img 文件夹里的一个名为 favicon.ico 的文件。可以自行更改，但要注意格式和尺寸。

---

## END
希望您能愉快的使用我们的项目<br>:-D
