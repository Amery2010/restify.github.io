# Restify 文档


## 更新文档

拉去最新的文档，只需要执行：

```bash
git clone --recursive git@github.com:amery2010/restify.xiangfa.org
cd restify.xiangfa.org
git submodule update --remote && git add _docs && git commit -m 'bump' && git push origin master
```

文档将自动使用 [GitHub Pages](https://pages.github.com/) 重建。

## 添加文档页面

要向网站添加文档，请添加相应的标题：

```text
---
title: [Page Title]
permalink: /docs/[page-id]/
---
```

然后通过在 `_data/docs.yml` 的相应部分添加 `page-id` 将页面添加到导航栏中：

例如：

```yml
...
- title: API
  docs:
    - server-api
    - [page-id]
...
```

## 本地运行

在开始之前你需要安装 Ruby 和 gem，然后：

```bash
# 安装 jekyll 和 bundler
gem install jekyll bundler

# 克隆项目
git clone https://github.com/Amery2010/restify.xiangfa.org.git
cd restify.xiangfa.org

# 运行 jekyll 及其依赖
bundle exec jekyll serve
```

## 设计

我们使用惊艳的 [jekyll-doc-theme by aksakalli](https://aksakalli.github.io/jekyll-doc-theme/) 作为我们的网站模板！
