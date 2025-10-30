---
title: hexo指令集
tags: [Hexo, 博客, 技术]
categories: [教程]
thumbnail: /images/hexo-logo.jpg  # 添加封面图
---
欢迎来到 [Hexo](https://hexo.io/)！这是你的第一篇文章。查看[文档](https://hexo.io/docs/)获取更多信息。如果在使用Hexo时遇到任何问题，你可以在[故障排除](https://hexo.io/docs/troubleshooting.html)中找到答案，或者在[GitHub](https://github.com/hexojs/hexo/issues)上向我提问。
<img src="![/images/tx2.jpg](https://img-blog.csdnimg.cn/direct/efd8105608be4a03ba9d1ef67ce41b6f.png?x-oss-process=image/resize,m_fixed,h_224,w_224)" alt="文章封面" width="80" height="80" style="border-radius: 50%; object-fit: cover;">
<!-- more -->

## 快速开始

### 创建新文章

```bash
$ hexo new "我的新文章"
```

更多信息：[写作](https://hexo.io/docs/writing.html)

### 运行服务器

```bash
$ hexo server
```

更多信息：[服务器](https://hexo.io/docs/server.html)

### 生成静态文件

```bash
$ hexo generate
```

更多信息：[生成](https://hexo.io/docs/generating.html)

### 部署到远程站点

```bash
$ hexo deploy
```

更多信息：[部署](https://hexo.io/docs/one-command-deployment.html)

## 常用命令
```bash
hexo clean; hexo generate; hexo server


# 生成静态文件
hexo clean
hexo generate

# 部署
hexo deploy

#一键部署
hexo clean
hexo generate
hexo deploy
# 测试 Git 连接
git ls-remote https://github.com/Cia011/Cia011.github.io.git
```


## hexo工作原理
本地Markdown文件 → Hexo生成静态HTML → 推送到GitHub → Cloudflare加速 → 用户访问  
静态生成： 运行 hexo generate 命令，Hexo会：读取Markdown文件,生成完整的静态HTML、CSS、JS文件到 public 文件夹
部署： 运行 hexo deploy 将 public 文件夹内容推送到GitHub仓库  
访问： 用户通过Cloudflare访问GitHub Pages服务提供的静态文件