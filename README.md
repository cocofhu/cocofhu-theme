# hexo-theme-cocofhu

cocofhu 个人站主题。首页开场、显示器和作品区写在主题里；「最近在做」「写作」从 Hexo `site.posts` 拉取。

## 在 Open Pages 里安装

1. 设置页安装来源填 `cocofhu/cocofhu-theme`
2. 把站点主题改成 `cocofhu`
3. 写 Markdown 文章后预览：首页列表应出现标题和链接

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
recent_limit: 6
writing_limit: 4
```
