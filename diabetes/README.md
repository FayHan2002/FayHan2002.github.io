# 糖尿病知识助手

为妈妈打造的移动端糖尿病知识网站。

## 如何添加新内容

### 添加文章

编辑 `data/articles.json`，按以下格式添加：

```json
{
  "id": 下一个编号,
  "title": "文章标题",
  "category": "medication/diet/exercise",
  "source": "来源名称",
  "sourceType": "book(基础知识) 或 platform(平台帖子)",
  "tags": ["标签1", "标签2"],
  "summary": "一句话摘要",
  "content": "完整内容（支持换行），如果是平台帖子可设为 null",
  "url": "外部链接（平台帖子必填，基础知识写 null）",
  "date": "YYYY-MM-DD"
}
```

### 添加平台链接

编辑 `data/links.json`，按格式添加。

- `platform` 可选值：`wechat` / `zhihu` / `xiaohongshu` / `bilibili` / `douyin`

### 添加常见问题

编辑 `data/faq.json`。

## 部署

推送到 GitHub 后自动部署到 `fayhan2002.github.io/diabetes`。
