# WHU CS 科研训练

本仓库是“WHU CS 科研训练”的公开课程网站与资料仓库，使用 MkDocs Material 构建并通过 GitHub Pages 发布。

## 本地预览

```bash
python -m pip install -r requirements.txt
mkdocs serve
```

## 构建

```bash
mkdocs build --strict
```

## 内容结构

- `docs/index.md`：课程首页与介绍
- `docs/schedule.md`：课程日历与课件索引
- `docs/assignments/`：课程作业
- `docs/faq.md`：常见问题
- `docs/lectures/`：从日历进入的各讲详情页
- `docs/assets/files/`：公开课件与课程文件

课程网站中的第三方论文和资源原则上只提供官方链接；版权归原作者或出版机构所有。
