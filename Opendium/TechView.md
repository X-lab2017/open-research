# 基于技术视角的开源纲目体系设计（Technical method）

本部分从技术手段与研究方法的视角来研究开源相关的课题，典型的分类体系包括：数据科学技术、软件工程技术、系统科学技术、社会学方法、经济学方法、管理学方法等。

# 一、数据科学与工程

  - 图算法-网络科学

    - 中心性算法

      - 算法：

        - 度中心性算法
        - 接近中心性算法
        - 中间中心性算法
        - pagepank算法

      - 问题：

        1. 对开发者，repo，organization的影响力进行分析

           - 简介：开源世界蕴含着社会关系，是由千万级开发者共同参与的世界，然后出现一个个仓库，组织等实体。社交网络中不是每个人和所有其他人都有直接联系，如果如此，便有了结构洞，即结构上的不完备。这种情况下，信息在网络中的流动受到其结构上的约束。每个人在网络中所能接触到的信息内容不再相同，传递和接受的时间也会出现差别。而在这些社会关系中，需要选择出重要的人或者重要的“桥梁”，帮助我们了解群组动态，例如可信度，可访问性，事务的传播速度等，目标：从不同维度领域对开发者、仓库和组织进行影响力进行分析排名

           - 相关论文：
             - Yan, D., Shao, Z., Zhang, Y., &#38; Qi, B. (2020). BurstBiRank: Co-ranking developers and projects in GitHub with complex network structures and bursty interactions. <i>Complexity</i>, <i>2020</i>. https://doi.org/10.1155/2020/7264396
             - Li, Y., Li, C., &#38; Chen, W. (2018). Research on Influence Ranking of Chinese Movie Heterogeneous Network Based on PageRank Algorithm. <i>Lecture Notes in Computer Science (Including Subseries Lecture Notes in Artificial Intelligence and Lecture Notes in Bioinformatics)</i>, <i>11242 LNCS</i>, 344–356. https://doi.org/10.1007/978-3-030-02934-0_32

    - 社团发现算法

      - 算法：

        - 三角形计数和聚类系数
        - 强连通分量算法
        - 连通分量算法
        - 标签传播算法
        - Louvain模块度算法

      - 问题：

        2. 开源社团（社区）发现

           - 简介：在社会网络中，容易形成一个又一个内部强联系群组。社团的形成在所有类型的网络中都很常见，在开源领域中尤其如此，每个项目或者几个项目都会形成一个完整的开源社区，形成各个角色都具有不可替代的作用。识别社团对于评价群体行为和突发现象不可或缺，也可以从识别的各个社区中发现新的知识领域和知识点，有助于发现最前沿的技术路线，也有助于归纳总结良好社区的特性特点，对开源社区的运营具有参考性理解。目标：从不同角度识别开源领域的开发者社区、技术社区、仓库社区。

           - 相关论文：
             - Javed, M. A., Younis, M. S., Latif, S., Qadir, J., &#38; Baig, A. (2018). Community detection in networks: A multidisciplinary review. In <i>Journal of Network and Computer Applications</i> (Vol. 108, pp. 87–111). Academic Press. https://doi.org/10.1016/j.jnca.2018.02.011
             - Rani, S., &#38; Mehrotra, M. (2019). Community Detection in Social Networks: Literature Review. <i>Journal of Information and Knowledge Management</i>, <i>18</i>(2). https://doi.org/10.1142/S021964921950019

  - 数据挖掘

    - 异常检测

      - 算法：

        - 统计学方法
        - 基于临近度的离群检测
        - 基于密度的离群点检测
        - 基于聚类的技术

      - 相关问题：

        4. github自动化协作行为识别

           - 简介：介绍：一些传统上手工执行的开发活动，例如代码提交、打开、管理或关闭问题，在许多OSS项目中日益受到自动化的影响。具体来说，此类活动通常由响应事件或在特定时间运行的工具执行。我们将这种自动化工具称为机器人，在许多与开发人员生产率或代码质量相关的软件挖掘场景中，为了将机器人的行为与个体行为区分开来，需要识别机器人的行为，因此识别机器人是很有必要的。目标:找到一种自动识别机器人和这些机器人提交的代码的方法，若可以需要根据它们的活动模式来描述机器人的类型。

           - 相关论文：
             - Dey, T., Mousavi, S., Ponce, E., Fry, T., Vasilescu, B., Filippova, A., &#38; Mockus, A. (2020). Detecting and Characterizing Bots that Commit Code. <i>Proceedings - 2020 IEEE/ACM 17th International Conference on Mining Software Repositories, MSR 2020</i>, 209–219. https://doi.org/10.1145/3379597.3387478
             - Golzadeh, M., Decan, A., Legay, D., &#38; Mens, T. (2020). <i>A ground-truth dataset and classification model for detecting bots in GitHub issue and PR comments</i>. https://doi.org/10.1016/j.jss.2021.110911
             - Wessel, M. (2020). Enhancing developers’ support on pull requests activities with software bots. <i>ESEC/FSE 2020 - Proceedings of the 28th ACM Joint Meeting European Software Engineering Conference and Symposium on the Foundations of Software Engineering</i>, 1674–1677. https://doi.org/10.1145/3368089.3418539
             - Golzadeh, M., Legay, D., Decan, A., &#38; Mens, T. (2020). Bot or not?: Detecting bots in GitHub pull request activity based on comment similarity. <i>Proceedings - 2020 IEEE/ACM 42nd International Conference on Software Engineering Workshops, ICSEW 2020</i>, 31–35. https://doi.org/10.1145/3387940.3391503

        5. github异常行为识别：

           - 介绍：GitHub上有不少账号存在刷star、刷issue的行为等，所谓刷star，刷issue行为就是存在与项目无关的issue或者对项目没有益处的issue，所谓刷star行为是指使用不符合正常情况下异常给项目点start，这些作假的start和issue会对开发者进行分类和识别会产生严重的干扰作用，也会阻碍其他开发者对这个账号产生正确的评判或者对这个仓库产生误解。这些操作可以通过图算法社团发现解决，也可以通过其他异常检测技术进行识别解决。目标：识别github中异常的账号和仓库。

           - 相关论文：
             - Lijun, Z., Wenzhong, Y., Tingting, Y., &#38; Xiang, J. (n.d.). 社交网络异常用户识别技术综述 仲丽君， 杨文忠， 袁婷婷， 向进勇. https://doi.org/10.3778/j.issn.1002-8331.1804-0374

    - 分类回归

      - 算法

        - k-近邻
        - 决策树
        - 贝叶斯分类
        - 逻辑回归
        - 支持向量机
        - 回归
        - 分类回归树

      - 问题：

        6. 对开发者、repo、issue，或者PR进行标签分类

           - 介绍：在开源协作领域，不同的开发者具备不同的角色，也具备不同的技术领域专长等，对这些开发者从不同维度进行分类有不少益处，可以用于向开发者推荐社区，帮助开发者发现感兴趣的社区项目，或者帮助开发者更好的融入社区，也可以用于向社区项目推荐人才，让社区针对性的吸纳领域人才和所缺乏的人才。同理对issue打标签可以更好的对issue进行分类，帮助社区核心维护者更好的进行项目管理。目的：从不同维度对开发者、项目、isssue，PR进行标签分类。

           - 相关论文：
             - Yang, C., Fan, Q., Wang, T., Yin, G., Zhang, X. hui, Yu, Y., &#38; Wang, H. min. (2019). RepoLike: amulti-feature-based personalized recommendation approach for open-source repositories. <i>Frontiers of Information Technology and Electronic Engineering</i>, <i>20</i>(2), 222–237. https://doi.org/10.1631/FITEE.1700196

    - 聚类

      - 算法：
        - K-Means
        - 凝聚层次聚类
        - DBScan

     - 问题：同2

    - 关联模式挖掘

      - 算法：
        - FP-growth 算法
        - Apriori算法
      - 问题：
        7. 开源知识图谱的构建、推荐

  - 推荐系统

    - 算法：

      - 基于内容推荐
      - 协同过滤推荐
      - 基于规则推荐
      - 基于效用推荐
      - 基于知识推荐
      - 组合推荐

    - 问题：

      6. 对PR推荐reviewer

         - 简介：基于PR的模型，广泛应用于分布式软件开发，为潜在的贡献者提供了一个极低的进入门槛(任何人都可以提交对任何项目的贡献，通过 提取请求)。同时，项目的核心团队必须作为代码质量的守护者，确保在拉出请求被合并到主要开发线之前被仔细检查。随着拉出请求越来越流行，对合格的评审人员的需求也在增加。GitHub促进了这一点，通过支持PR和Comment的众包，以实现不仅仅是项目的核心团队还有程序员之间的沟通交流，这是程序员社会协作理念的一部分。然而，能够有更多潜在的评审者可以审阅并不一定意味着更容易找到正确的问题（“大海捞针”的问题）。如果不受监督，这个过程可能会导致沟通过载和会推迟PR请求处理。目的：研究不同的推荐方法是否以及如何适用于为pull-request推荐reviewer人员，以及如何提高推荐性能。

         - 相关论文：
           - Yu, Y., Wang, H., Yin, G., &#38; Wang, T. (2016). Reviewer recommendation for pull-requests in GitHub: What can we learn from code review and bug assignment? <i>Information and Software Technology</i>, <i>74</i>, 204–218. https://doi.org/10.1016/j.infsof.2016.01.004

# 二、软件工程

  - 软件开发领域
    - 软件需求：需求获取、需求分析、需求描述、需求验证、需求变更、需求控制等
    - 软件设计：技术/框架选型、结构/架构设计、用户界面设计、组件/接口设计等
    - 软件构建：程序编码、单元测试、集成测试的过程
    - 软件测试：用事先设计的好的测试用例检测软件错误和失败
    - 软件维护：根据反馈意见和新需求做软件的修改、测试、更新
    - 软件配置管理：简单地理解就是版本控制，是一个时间点上所有与软件相关的信息的快照
    - 软件工程管理：启动、规划、实施、监控、结束等
    - 软件工程过程：软件生命周期过程本身的定义、实现、评估、管理、变更和改进
  - 工程实践领域
    - 软件工程模型与方法：在软件的生产与使用、退役等各个过程中的参考模型的总称，诸如需求开发模型、架构设计模型等都属于软件工程模型的范畴；软件开发方法，主要讨论软件开发各种方法及其工作模型
    - 软件质量：目标、评审、总结报告等
    - 软件工程职业实践：软件工程师应履行其实践承诺，使用软件的需求分析、规格说明、设计、开发、测试和维护成为一项有益受人尊敬的职业；还包括团队精神和沟通技巧等内容
  - 基础知识领域
    - 软件工程经济：研究为实现特定功能需求的软件工程项目而提出的在技术方案、生产（开发）过程、产品或服务等方面所做的经济服务与论证，计算与比较的一门系统方法论学科
    - 计算基础：解决问题的技巧、抽象、编程基础、编程语言的基础知识、调试工具和技术、数据结构和表示、算法和复杂度、系统的基本概念、计算机的组织结构、编译基础知识、操作系统基础知识，数据库基础知识和数据管理、网络通信基础知识、并行和分布式计算、基本的用户人为因素、基本的开发人员人为因素和安全的软件开发和维护等方面的内容
    - 数学基础：集合、关系和函数，基本的逻辑、证明技巧、计算的基础知识、图和树、离散概率、有限状态机、语法，数字精度、准确性和错误，数论和代数结构等方面的内容
    - 工程基础：实验方法和实验技术、统计分析、度量、工程设计，建模、模拟和建立原型，标准和影响因素分析等方面的内容
  - 问题：
    7. 开源社区生命周期度量
       - 简介：来自软件用户的反馈，如错误报告，在软件项目的管理中是至关重要的。在GitHub中，反馈通常表示为新问题。通过归档问题报告，用户可以帮助识别和修复bug，记录软件代码，并通过特性请求提高软件质量。这些都可以通过github的issue标签观测到，通过调查热门项目中与用户行为的重要程度来评估各种角色在GitHub中的重要性，并对用户行为标注并归纳开源社区的生命周期。目的：研究开源协作的一些特点。发现不同的开发模型，对应于项目的生命周期，可以帮助决策者更有效地管理和分配项目资源，甚至减少软件故障。
       - 相关论文：
         - Liao, Z., He, D., Chen, Z., Fan, X., Zhang, Y., &#38; Liu, S. (2018). Exploring the Characteristics of Issue-Related Behaviors in GitHub Using Visualization Techniques. <i>IEEE Access</i>, <i>6</i>, 24003–24015. https://doi.org/10.1109/ACCESS.2018.2810295
         - Saini, M., Chahal, K. K., Verma, R., &#38; Singh, A. (2020). Customer reviews as the measure of software quality. <i>IET Software</i>, <i>14</i>(7), 850–860. https://doi.org/10.1049/iet-sen.2019.0309

# 三、系统科学

可从github的devOps视角和github网站建设视角考虑

待补充~

