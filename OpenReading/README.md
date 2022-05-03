### OpenReading

**OpenReading** 是 OpenResearch 项目下的一个论文分析与阅读模式（包括十大步骤），基于 GitHub 上的 Discussion、Issue、PR、Wiki 等功能，及其这些实体之间的转化。目的是迭代一个开放、高效、能够不断沉淀的分享模式。

一张图展示就是：

<div align=center>
<img src="https://user-images.githubusercontent.com/15010826/166209838-d3182d7d-2fda-4642-808a-01bde72b8f6d.png" width="600px">
</div>

**<p align="center">GitReading 十步法</p>** 

#### 1、提出候选论文

通过 `OpenResearch` 仓库上的 `Discussion` 或 `Issue` 提出想要阅读与分享的候选论文，其中：
- 如果 idea 还不成熟，可以用在 `Discussion` 下面进行预先讨论，成熟后，通过 GitHub 上的 `Discussion ➡️ Issue` 功能进行转换
- 有成熟 idea 的，直接用 `Issue`进行提议

#### 2、填写 RPP 模板

用 `Issue` 进行提议的时候，可以遵照一个 `OpenPro` 的模板，进行结构化的描述，方便丰富待分享论文的上下文。

✳️ **`Reading plan proposal, OpenPro`** 模板（9要素）：
- **论文题目**（Title）：论文完整正式的标题
- **作者与机构背景**（Author and affiliation）：主要作者与作者所属机构或实验室的背景信息
- **发表年份**（Year）：正式发表或公开上传的年份
- **会议或期刊名称**（Conference or Journal）：论文发表的会议或期刊名称
- **级别**（参照 CCF 级别）（Ranking）：如会议和期刊列入 CCF 的分级中，可以标注上
- **分类标签**（参照 Opendium）（Lable）：参照开源纲目中的分类体系
- **论文链接**（Link）：论文全文的链接信息，或放在实验室的 OSS 存储服务上
- **选题原因**（Select reason）：简单描述下选题的原因，特别是和实验室研究方向的关联
- **相关背景补充**（可选）（Background）：其他可选的背景补充信息

#### 3、深度阅读、动手实践
- 根据一般科研论文的阅读方法 [**一个参考📒**]  [**另一个参考📒**]  [[**子豪兄惊喜版😎**](https://www.bilibili.com/video/BV15w411Z7LG?p=11 "子豪兄版")]
- 必要的实验复现，或此基础上的修改与优化等工作
- 阅读过程当中，追踪到的新论文，可以添加到论文列表库中 [[📚点击这里](https://github.com/X-lab2017/open-research/blob/main/openlist.md) "论文列表")]
- 做好初步思考总结，笔记、PPT 等工作

#### 4、内部分享讨论
在 X-lab 的组会等活动上进行正式的分享，同时也锻炼自己的讲述表达能力 语雀的图床

分享过程会录制，并上传到 X-lab 的 B 站公众号上。[[**进入🎥**](https://space.bilibili.com/510793367 "B站视频")]

#### 5、会前会后撰写分享报告

可以将此项工作前置，而不用等到分享结束。尽早起步，不断迭代，是不二的法则，还可以及早收获老师同学们的反馈（需要自己主动点）。[[**好的参考1📒**](https://www.yuque.com/shibudengqinsheng/ggwvkm/eri2s3 "一个参考")][[**好的参考2📒**](https://www.yuque.com/tyn1998/blogs/cs1unx "另一个参考")]

✳️ **`Reading plan proposal, OpenRep`** 模板（6要素）：
- 步骤 3 中 OpenPro 的引用
- 论文摘要（Abstract）
- 主题内容（Main content）
- 分享时的讨论（Disscususion）
- 外部讨论内容（可选）（Open discussion）
- 思考与启发（Inspired thinking）

#### 6、发布分享 RP，收获外部反馈，并持续迭代

- 用自己喜欢的工具或平台进行发布，例如 X-lab 采用的`语雀`、个人博客等 [[**一个博客参考📒**](https://blog.frankzhao.cn/ "一个博客参考")]
- 将自己的内容导出为 Markdown 格式 [[**还不会 Markdown❓**](https://www.bilibili.com/video/BV1Yb411c7Hi?spm_id_from=333.999.0.0 "学习 Markdown")]
- 稍微修改一下导出的 Markdown 格式，使其符合博客引擎的要求
- 自己本地先看看博客渲染效果，例如使用 `Typora`（可以吗？）

#### 7、正式提交 PR 到仓库中
- 没有问题后，将这篇报告通过 PR 的形式贡献到仓库的 `open-research/OpenReading/` 目录下
- 触发 GitHub 的 Action，自动将 PR 中的 Markdown 渲染为文章，将此 PR 部署到线上，并由 bot 给出对应链接（就像Frank在OpenGalaxy中做的那样）

遗留问题，图床需要统一确定一个：
- 语雀的图床
- 阿里云 OSS 的图床

#### 8、根据反馈优化 OpenRep

- 其他读者点进链接，阅读排版精美的 RR，并在 PR 中给出建议
- 作者做出相应修改，push 新的 commit 上来，再次触发 Action
- 并且由于 PR 中可以看 diff，作者改了哪些地方将是一目了然
- 完善好后，合并 PR 到 main 分支，触发另一个GitHub Action 进行更新
- 可以不断迭代

#### 9、多平台宣传

看准时机后（例如），就可以在各大媒体平台上进行宣传了。
- 微信号
- 微博
- 知乎
- Weekly newsletter of X-lab：https://www.getrevue.co/profile/x-lab
- 国内不知道有没有上述这样的宣传平台

#### 10、发起新的工作

通过上述这些内容，可以帮助你找到新的切入点与后续工作机会，包括：
- 找到新的研究论文或专著进行阅读 [[📚点击这里](https://github.com/X-lab2017/open-research/blob/main/openlist.md) "论文列表")]
- 收获实验室老师同学们的反馈，启发进一步的工作
- 大家形成一些共识，继续往前走

💡 本文只是给出的一个论文阅读与研究的框架，不必完全按照上述步骤，但将会是我们不断迭代与完善的一个最佳实践，相信共同的智慧，会一起陪伴在于大家的科研道路上，research in public 将会是我们的一个新尝试~ 

