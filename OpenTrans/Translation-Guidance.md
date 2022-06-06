# 翻译流程

### 1. 选择一篇要翻译的文章
- 文章选定后，在[语雀知识库](https://xlab2017.yuque.com/books/share/a8959c62-a36d-41a3-b708-f253f32dddec?#)中建立一个新文档，以要翻译的文章题目命名
- 在[open-research](https://github.com/X-lab2017/open-research) 仓库下提交一条新的 issue，使用 Paper Translation 模板，填写以下字段：
    - Title：翻译的文章题目
    - Source Link：原文链接
    - Translation Link：译文（语雀文档）链接

### 2. 开始翻译
- 在 [X-Translation](https://github.com/orgs/X-lab2017/projects/5/views/1) 下新增一条翻译任务，追踪翻译进度
- 翻译过程中，可以借助 DeepL 进行和自动化翻译和审查
- 翻译过程中，遇到问题可以在对应的 Issue 下追踪，翻译进度在 Projects 看板下追踪

### 3. 初翻完成
- 全文翻译好之后可以自我阅读一遍，保证语句通顺流畅
- 提交一个 PR 到 [Table ](https://github.com/X-lab2017/open-research/blob/main/OpenTrans/Table.md)文件，新增一条记录，填写以下字段：
    - 序号：自加一
    - 原文：原文的文章名称，并添加文章地址的超链接
    - 作者：原文的作者，有多位作者可以只填写一作
    - 译文：译文的语雀链接，用 “Link” 加上超链接表示，防止过长
    - 译者：译者姓名
- 可以在 PR 中指定一个审稿人来 review 你的翻译，也可以在这个过程中自己进行二审，修订一些小细节
- PR 合入之后，状态设置为 `5-翻译完成`，文章翻译完成。🎉🎉
