# Learning Notes

这是 Learning Web 使用的个人笔记仓库。应用代码单独保存在 [learning-web](https://github.com/DjTaNg-404/learning-web)。

应用在用户点击同步后写入 `notes/<topic-id>.md`，每次同步保留 Git 版本历史。初始化不会上传本地学习示例。

每篇笔记使用以下开放格式：

```markdown
---
{"id":"topic-id","title":"学习主题","description":"主题说明","tags":["标签"],"format":"learning-web/v1"}
---

# 我的理解

这里是确认后的 Markdown 笔记。
```

头部为 JSON 形式的 YAML frontmatter。保留文件名和 `id` 一致，便于应用从仓库恢复主题。

API Key、订阅授权令牌、GitHub Token、运行数据库和环境配置存放在应用运行环境中，不进入这个仓库。聊天历史由应用后端保存，也可以从应用导出 JSON 归档。

