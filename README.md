# hexo-theme-cocofhu

cocofhu 个人站主题。首页开场、显示器和作品区插画写在主题里；「正在进行」三段文案和「最近在做」来自主题配置（Open Pages 设置里可视化编辑）；「写作」从 Hexo `site.posts` 拉取。文章页和首页同一套近黑阅读皮。

## 在 Open Pages 里安装

1. 设置页安装来源填 `cocofhu/cocofhu-theme`
2. 把站点主题改成 `cocofhu`
3. 在主题设置里编辑「正在进行」（固定三条文案）和「最近在做」：选中文字可加 hover 说明
4. 写 Markdown 文章后预览：「写作」列表出现标题和链接

本地 Hexo：

```bash
npm i hexo-theme-cocofhu
# 或 git clone 到 themes/cocofhu
```

`_config.yml`：

```yaml
theme: cocofhu
```

主题配置（`_config.cocofhu.yml` 或主题 `_config.yml`）：

```yaml
writing_limit: 4
links:
  github: https://github.com/cocofhu
  rss: atom.xml
  email: ""
work:
  title: 正在进行
  items:
    - date: "2026 · PRODUCT"
      title: SkillHub 研发负责人
      url: https://skillhub.cn/
      link: 打开 skillhub.cn
      excerpt: 面向中国用户的 **AI Skills 社区**——帮 Agent **搜索、安装、调用** Skill。
recent:
  title: 最近在做
  lede: 看看我在做什么
  index_label: 01 NOTES
  items:
    - date: "2026 · 09"
      title: Hello Open Pages
      tag: WELCOME
      url: ""
      excerpt: 在这里用 Typora 式所见即所得写 Markdown。
      hovers:
        - match: Typora 式
          tip: 对对对就是这样，太对了
```
