---
title: README.MD
date: 2020-01-30 19:25:27
tags:
# index_img: /img/example.jpg
---

欢迎来到我的博客,
在这里简单介绍下本站所用的开源项目.
<!-- more -->
### Hexo 博客框架
一个基于 Node.js 的博客框架, 可以将 MarkDown 编译为静态页面.

### Fluid 主题
在 Fluid / Butterfly / NexT 中选择了它, Burrerfly 的效果很酷, 但可能是绑定了过多事件监听的缘故(瞎猜), 导致 CPU 占用不小, 而且没有标题的导航, 而 NexT 过于朴素, 最近很喜欢大阴影, 所以选择了 Fluid.

### GitHub Pages 页面托管
可以免费托管静态页面 感谢 GitHub, 有了 Hexo + GitHub Pages 建博客的成本低了许多.抛去域名就是0成本.

### Cloudflare CDN
由于国内运营商对 GitHub 有不同程度的屏蔽, 因此套上一个免费的CDN, 略微体升访问速度的同时, 降低被墙的风险.

### Gitalk 评论系统
基于 GitHub issues 的评论工具.
很久没有接触博客这快, 评论系统有了很大的变化, 过去的多说 / 畅言已接近放弃维护, 又有审查的风险, 现在都采用基于 GitHub issues 的技术, 原理是在 git 根据每篇文章的唯一标识(这里用标题)在仓库中开辟一个 issues, 大家的回复就相当于在相应的 issues 回复, 再抓取其中的内容到自己的博客, 这样理所当然是支持 MD 评论的.
不得不再次感慨技术的变化, 以及伟大的 GitHub 让我们薅羊毛.