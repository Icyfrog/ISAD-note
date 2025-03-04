## 第一章 互联网时代的软件工程
- 1 互联网时代的软件系统
    - 1.1 互联网时代软件特点
        - 业务和信息紧密融合
            - 复杂的业务和用户，业务快速变化，移动应用的发展，线上线下融合的一体化进程加速
        - 规模大，并发性高
            - 软件分布和使用没有时空约束，用户数量庞大
        - 周期短，更新快
            - 生存周期短，开发、发布、更新都要敏捷快速
        - 开放，普世环境
            - 不同的接入方式为不同设备和网络等用户提供服务，同时通用的web浏览器可以与不同平台用户交互
    - 1.2 互联网时代的软件挑战
        - 如何实现以用户为导向个性化软件需求
            - 不能指望用同一套逻辑应对所有的客户需求，即使提供的是同样的产品或服务
        - 如何构造以柔性可变为核心的软件形态
            - 不能事事都通过软件开发人员去修改软件。“柔性”软件以相应用户的业务流程调整请求
        - 如何完成以快速敏捷为特征的软件开发过程
            - 越来越多的功能业务趋于“软件化”，人们趋于改变软件来适应硬件，软件也会在原有应用范围边界，或者超过边界的情况下使用
        - 如何适应以普世移动为特点的软件开发和应用环境
            - 越来越多的设计开发建模测试等等都在互联网环境上开展。
- 2 互联网时代的软件工程思想
    - 互联网时代的软件工程方法从四方面体现：
        - 软件需求
        - 软件形态
        - 开发过程
        - 软件验证
    - 2.1 覆盖全生命周期动态获取的软件需求
        - 互联网环境下没有了时空约束，软件需求方面的变化主要有：
            - 需求主体：不是确定的个体或组织，而是不确定的个体组织而成的群体
            - 需求获取：不是静态定义规约，而是延伸到系统运行时的动态获取
                - 软件开发的各个阶段的产物，都是软件需求动态获取的可能途径
            - 需求满足：不是一次性的功能开发，而是运行时软件的自适应和是持续演化
                - 软件需求由一次性的测试提交，转化为覆盖全生命周期的多次迭代和持续交付
    - 2.2 基于流程的网络服务动态集成（形态）
        - 软件形态的主要变化：
            - 软件构建：从功能构建构造，转变为以业务为核心的多功能处理流程
            - 组装方式：从功能组装集成，转换为多个服务交互实现动态组合
            - 运行环境：从环境静态预设，转换为面向情景感知的软件自适应
                - 在动态的互联网环境下，软件自身的自治性要增强，实现对环境状态的动态感知，并能够调整自身结构，产生动态行为以适应外部环境
    - 2.3 基于敏捷和增量迭代的协同软件开发过程
        - 软件过程从循序渐进的阶段推进方式，向基于敏捷和紧密协同的软件开发过程转移
        - 体现的要点：
            - 过程推进：阶段循序的渐进开发模式 --> 各阶段便捷模糊的敏捷模式
            - 开发方式：系统开发结果的整体提交 --> 不断迭代的增量开发及提交方式  （典型的项目管理工具：Scrum框架）
            - 团队协作：各团队注意接口的分工合作 --> 各团队界限模糊的协同融入方式 （流行举例：DevOps）
    - 2.4 用户体验为中心的软件验证演进
        - 由于软件形态的变化，软件验证已经从测试为主，转变为以用户体验为中心，主要体现在：
            - 验证目标：以功能满足为核心的软件测试，转变为以用户体验为核心的产品验证；
            - 验证方式：以软件上线的全面测试，转变为软件上线运行后的渐进优化；；；一次全面测试往往不能满足集成需要，因此验证方式为，从软件运行状态出发，实现软件系统的持续治理
            - 验证内容：以软件代码的需求覆盖性测试，转变为运行数据挖掘分析后的模型一致性验证；；；是以用户体验为核心，通过用户反馈对产品进行验证
- 3 互联网时代的软件工程方法框架
    - 互联网环境下的软件工程方法框架几包含三个维度：
        - **过程维度**：覆盖全生命周期的持续优化框架是当前软件领域的关注方向
        - **形态维度**：微服务和容器的结合使开发人员的新宠
        - **管理维度**：Scrum + DevOps 结合的软件项目管理模式逐渐成为主流
    - 3.1 模型驱动的全生命周期业务建模及转换（过程维度）
        - 业务建模包括多种形式
            - 功能建模、数据建模往往是建立软件系统的起点
            - 业务流程建模成为你主流的业务建模方式
            - 基于数据的视角思考成为当前的热点
        - （1）业务建模
        - （2）模型驱动体系结构（MDA）
    - 3.2 基于服务的软件动态构造（形态维度)
        - 面向服务的架构（SOA）是以业务为导向的一种软件系统分析和开发方法，通过应用Web服务创建软件解决方案
        - Web服务发展迅速的原因
            - 采用广泛部署的**通信协议**（如http）传输基于XML编码的纤细是的跨企业的分布系统间的通信和互操作成为可能
            - 基于文档的***消息模型**更适合不同类型的应用之间对松耦合的要求
            - Web服务的出现使得业内首次拥有了一个建立在真正支持互操作性的开放标准基础上的应用解决方案
        - （1）服务组合
        - （2）轻量级Mashup
        - （3）最终用户开发
    - 3.3 敏捷化的软件项目开发及运维（管理维度）
        - 敏捷软件开发模式缩小了**需求和开发**之间的第一个隔阂
        - 敏捷软件运维模式DevOps所线了**开发和运营**之间的第二个隔阂
        - （1）敏捷软件开发与Scrum
            - 敏捷软件开发强调以人为本，快速响应需求和变化，把注意力集中到主要目标——可用软件上，在保证质量的前提下，适当文档，适度度量
        - （2）软件运维与DevOps
            - 敏捷软件运维将开发与运营一体化，形成DevOps(Development & Operations)
            - DevOps是软件开发、运营和质量保证三个部门之间的沟通、协作和集成所采用的的流程、方法和体系的一个集合，包括：
                - 持续集成与发布
                - 自动部署
                - 监控
                - 日志分析
## 第二章 互联网时代的软件实现模式
- 目录
    - 1 软件的三种开发模式
        - 定制开发-套件实施-模型驱动架构
    - 2 复杂软件的业务建模
        - 业务模型-业务建模及软件建模-业务架构
    - 3 持续演化的软件架构
        - 软件架构演化-多层架构-微服务架构
    - 4 互联时代的软件过程
        - 开发实施过程-工具支持-角色职责
- 1 软件的三种开发模式
    - 软件系统的开发实施过程覆盖了从业务问题到可运行系统之间的软件各阶段
    - 1.1 基于定制开发模式的软件架构
        - 顾名思义 为企业或者组织“定制”
        - 定制的软件系统一般含有高事物量的大系统，或者具有特殊业务需求的系统
        - 定制开发 不考虑时间成本和质量等问题，解决客户提出的所有业务需求
        - 传统的软件开发大都属于定制开发模式
        - 优势：理论上可以满足所有的业务需求
        - 劣势：人员、周期
    - 1.2 基于套件模式的软件系统实施
        - 基于商业化平台，通过业务模型导引下的数据和功能位置，搭建可用系统的过程
        - 在这些软件系统套件基础上，覆盖企业业务需求的业务蓝图，指导软件系统的功能配置和界面设计，是设计和实施大型系统的重要策略
        - 业务蓝图就是业务参考模型，描述了企业业务的四个方面：事件、功能（任务）、组织、交互
        - 业务蓝图的目的是将复杂的业务进行流线式的过程描述
        - 优势：开发周期短、开发成本较低、软件质量较为稳定
        - 劣势：受到软件已有功能和架构的显示，用户的部分特别需求往往难以得到完全满足
    - 1.3 业务模型驱动的软件架构模式
        - 业务模型驱动的IT架构方式是当前软件系统分析与设计的重要发展方向
        - 模型驱动架构模式，就是指在构建的业务模型基础上，通过模型驱动的转换，实现软件的架构，进而构造出可运行的软件
        - 在业务模型基础上构造的高度集成的软件系统，不仅会改善 整体业务，而且可以使软件更容易调整并适应将来的业务变化
        - 还有两幅图，看的有点不懂，但是感觉会是重点hhh
- 2 面向复杂软件构造的业务模型
    - 软件系统和业务模型密不可分。构造软件的前提是对涉及到的企业业务状态进行建模和分析。建模 就是 标准而规范的描述手段
    - 2.1 业务建模概述
        - 业务建模是对于企业业务的某些方面进行的描述
        - 业务模型是针对业务功能的抽象描述，是复杂现实世界问题的简化，建立的标准而规范的描述手段和统一试图
        - 建模需要定义模型的目的、范围、视角以及粒度
        - 业务模型在不同角度下有不同的分类
    - 2.2 业务建模方法发展
        - 基于功能
            - SADT结构化分析与设计方法和IDEF功能分解法
            - 存在主要问题：功能分解法基本组件只有一个，有很好的通用性，但是缺乏丰富的语言表述能力
        - 基于过程
            - 面向过程的经典方法有：数据流图，状态-变迁图
            - 基于 数据 活动 事件 状态 业务流程建模，四种实现过程
            - 集成化建模（多视图建模）
        - 基于服务
            - 面向服务的建模更多的是面向软件的构造和运行开展建模， 标准SOA服务或者RESTful服务
        - 基于大数据
    - 2.3 业务架构
        - 企业架构包括 业务架构 信息架构 技术架构等部分，业务架构是上层指导性架构，其他的创建和分析的基础
        - 业务架构的三个层次
            - 视图：业务模型由视图组成。视图表现业务的特定属性，抽象描述，忽略无关细节
            - 模型图：视图由多个模型图组成。每个模型图表达了业务结构的特定部分或者特定的业务状态。引入不同图标表达业务模型视图的不同方面或机制
            - 业务对象及关联：用不同的对象表征业务概念，关系使不同概念之间相互关联
        - 业务模型具有 多视角、多层次、复杂相关、时序依赖等特点，企业的业务建模要遵循一定的原则：
            - 分离，业务各个侧面分离
            - 分层，不同抽象成都，反应系统不同层面
            - 分解，根据总体目标，将功能活动逐步分解为各个组件，逐步细化
            - 一致性，各组件语义语法保持一致
            - 模块化，构建独立的各个模块
            - 通用化，提高模型的通用成都，定义接口，协议，构建等等
            - 功能与行为分离，功能考虑做什么，行为是如何去做，别陷入细节泥潭
            - 活动与资源解耦，活动描绘需要做的事情，资源描绘执行或等的人或设备，解耦可以提升企业执行的柔性
            - 分离，分解，分层，一致性说的是建模方法。模块化和通用性说的是工程化要求，最后两个表述容易出现的问题
    - 2.4 业务建模和软件建模
        - 软件系统建立基础性业务模型有以下好处：
            - 业务逻辑可以系统间重用
            - 系统之间更易于整合，便于信息交换和共享
            - 软件系统自然成为总体业务的一个内在组成部分，为业务提供足够的支持并提高工作效率
            - 系统更容易随着业务模型的变化进行相应的升级和修改，大大减少了软件系统维护和持续更新成本
            - 业务模型和软件模型的区别：40页 业务模型更高层，软件模型属于技术层面，更底层
- 3 持续演化的软件架构
    - 3.1 软件架构的演化阶段图 ppt43
    - 3.2 MVC架构，经典多层架构
    - 3.3 以业务为中心的微服务架构
    - 微服务架构
        - 微服务是一种思想：开发时便要考虑到运维需要，运维时实现软件灵活变冷
        - 微服务的架构风格
        - 微服务架构的主要特征
        - 微服务的优点：弹性，易扩展，简化部署，技术异构型，与业务组织结构相匹配，可组合，可代替性好
        - 实现微服务架构的主要要点
        - 单体架构和微服务架构的区别
        - 微服务带来的主要问题
- 4 面向互联网的软件过程
    - 
        
## 第三章 业务流程建模方法
### 1 基于人物的过程建模方法
- 功能分解图-活动图-角色行为图-人物的执行控制
### 2 基于数据的过程建模方法
- 数据分类-数据流图-组织建模
### 3 基于状态的过程建模方法
- 离散事件动态系统-经典Petri网-高阶Petri网-Petri网仿真实例
### 4 基于消息时间的过程建模方法
- 实践过程链EPC-规则语义-ARIS建模实例
### 5 小结

- 1 基于任务的过程建模方法
    - 基于任务的流程建模，就是基于功能的建模方法，是最为基本的业务建模描述方法，包括
        - 基于功能结构的任务划分
        - 面向执行的活动系列
        - 控制逻辑的描述
    - 介绍几个图
        - 功能分解图
        - 基于时序的活动描述
        - 角色行为图
        - 任务划分
    - （1）功能分解图
        - 本质：自顶向下
        - 将复杂系统分割成小的模块，分层组织功能模块
        - 模块按照**高内聚，低耦合**的方式设计并组织
        - 功能分解图就是 整个系统分解子系统，再分解功能，再分解为子功能
        - 在端点或者叶子节点上的模块包含执行程序功能的确切算法
        - 高层模块调用底层，底层不会调用高层
        - 模块下有带弧度的箭头，表示循环调用
        - 如何划分任务，是功能任务分解的主要问题
            - 根绝角色活动划分（以角色的任务区分为主）
        - 软件系统划分还有：
            - 根据信息对象的划分（面向信息服务的开发方式）
            - 根据操作的任务划分（具体功能的划分）
            - 根据流程的任务划分（子系统的划分）
    - （2）基于聚类的任务划分
        - 如果角色尚未确定，任务的划分方式主要可以从和相关业务要素的关系进行划分
        - 比如UC矩阵
        - 主要过程包括
            - 任务相关性矩阵构建
            - 构造聚类谱系图
            - 分解演化相关人物，重新建立任务关系
    - （3）基于时序的活动描述
        - 活动图描述的是对象活动的顺序关系所遵循的规则，描述对象之间传递的操作，多个组织或者角色的描述方式，一般采用带用到的活动图进行描述
    - （4）角色行为图
        - 角色行为图RAD(Role Activity Diagram)是一种常见的流程图形化描述方法，主要用在组织建模中
        - RAD基于活动的执行时序描述不同组织的交互活动。
        - 它特别擅长强调流程中的角色职责
        - RAD的主要特点
            - 按角色分解流程
            - 基于角色状态描述的流程目标
            - 按时序执行的活动
            - 关注角色的交互作用而不是形式
            - 体现企业的经营规则
        - RADD图评价
            - RAD由传统的基于活动的流程图派生而来，增添了包括状态和控制等元素，状态表明活动的原因和结果，控制表示路径选择
            - RAD表示法扩展了基于活动的流程表示，角色交互明晰化，也增加了表示的复杂性，因此不便于表达交互特别复杂的流程
            - RAD方法不足之处在于不具有模型分解的能力
            - 可以通过非层次划分，通过嵌套，一个自有的活动可扩展为新的RAD图，角色和活动可以重新展开
### 3 基于状态的过程建模方法
- Petri网理论(P8)
    - Petri网主要用途
        - 系统仿真：系统分析与评估的系统仿真
        - 数字分析：可以通过结构变化描述系统的变化，支持DEDS形式的数学描述与分析
        - 系统性能分析：直接从可视化模型汇总产生DEDS监控编码，进行系统实施控制
        - 还可以转化为其他的DEDS模型，如马可夫链等
- Petri网在计算机软件汇总的应用：11
- Petri网的主要特点 12
    - 简化细节 易于理解
    - 精确描述条件的依赖于不依赖
    - 方便建模和仿真
    - 更适合描述并发和冲突
- 经典Petri网理论
    - 基本元素
        - 库所 Place 圆形节点
        - 转移 Transition 方形节点
        - 连接 Connection 库所和转移之间的有向边，具有方向，用有箭头的线表示
        - 托肯 Token 是库所汇总的动态对象，可以从一个库所移动到拎一个库所，用实心的圆点表示
        - **库所**代表条件，缓存，渠道，地理位置或者状态
        - **转移**代表活动、动作、传输或者转换
        - **token**代表对象，信息或者对象的状态
        - 过程的状态用库所中的token，状态之间的变换用转移来表示
    - 经典Petri网规则：
        - 连接有方向，上面可以标出权重
        - 库所和库所不能直接相连，转移和转移也是，同时不能有孤立的节点
        - 一个库所可以有任意数量的托肯
    - Petri网的描述定义
        - 输入库所 input place：对于转移来说，token从输入库所转进来
        - 输出库所 output place：对于转移来说，经过转移的手，token转到输出库所中
        - 对于转移来说，必须与它相连的所有输入库所都有token，才能激活转移
    - Token转移的例子
        - token点火向不同的转移具有冲突和不确定性
    - Petri网的行为规则
        - 一个转移的所有输入库所都有token，那么转移就是被允许的，输入库所token被消耗，输出库所产生token
        - 转移必须是完整的，不能一个转移发生了一半
        - token数量可以不守恒
        - 如果多个转移都有被允许的可能，那么转移发生的顺序就没有定义，可以认为是并发的
        - 多个转移争夺一个token被称为**冲突**，冲突的结果是随机的
        - Petri网是静态的，工作中时不会突然增加一个转移或者库所；来改变Petri网的结构
        - 转移生在发生的时候，Petri网不算是确定的状态，一个转移结束、下一个转移等待发生的时候才有确定的状态
    - Petri状态
        - 当前状态：Petri网的状态由库所中托肯的当前分布情况确定 
        - 可达状态：通过一系列激活转移的点火，从当前状态可以达到的状态
        - 死状态：没有转移能激活的状态
    - Petri网定义为**五元组**（库所、转移、输入函数、输出函数、初始状态）。任何图都可以映射到这样一个五元组上 ∑ = ( P ， T ，F ， K ， M0 ) 
        - P 库所集合 圆圈 代表系统状态
        - T 转移集合 空心矩形 系统的动作或者操作
        - F P->T 资源的输入流
        - K T->P 资源的输出流
        - M0 Petri网∑的初始状态
        - Token是工作对象，转移是网络中的控制点
    - Petri网的工作流网构造：**PN=(P,T,F,W,M)**
        - (P,T,F)是基网，此时F为不区分F,K的统一流关系表述
        - W是有向弧的权重函数
        - M为状态，是一个多维向量的集合，M(p)表示库所P中的token数
        - 对于t属于T，·t表示转移t的所有的输入库所的集合
        - 对于t属于T，t·表示转移t的所有的输出库所的集合
        - *有颜色？* 在PN终止库所O和开始库所I之间插入一个转移t*并添加相应的连接弧，构成PN的扩展网络
    - 工作流网
        - 大概就是画图画的
    - demo 
        - P43 P35 P36
    - 高阶Petri网
        - 经典Petri网建模方法有缺点
            - 没有测试库所中零token的能力
            - 模型容易变得很庞大
            - 模型不能反应时间方面的内容
            - 不支持构造大规模模型，如自顶向下或自底向上
        - 高阶的Petri网对以下方面进行了扩展
            - token着色：token有了颜色，代表token建模对象的具体特征
            - 时间：每一个token有一个时间戳，转移决定生产处的token
            的延迟，并增加时序逻辑的定义
            - 层次化：构造一个与分层数据流图类似的复杂性建模机制(为Petri网增加了结构信息的方法)
        - 高阶Petri王的拓展步骤
            - 采用颜色进行拓展，加入产生的token数目，token的值，有一个前提条件（可选）
            - 时间的拓展：每一个token都有一个时间戳
            - 对复杂的Petri网添加了结构信息的方法
    - 基于Petri网的过程建模方法 **第二次作业的重点**
        - Petri网建立步骤：
            - 根据状态和事件的定义，确定系统的状态集和事件集。
            - 确定系统中状态与事件的关系
            - 讲库所和转移对应起来，建立Petri网模型图
            - 根据系统情况，决定Petri网模型图的初始状态，确定初始状态的下个状态的token数
            - 基于初始状态判断哪些事件可以被激发，当模型激活后，模型状态图将发生变化，又引起一些事件被触发
    - 给的两个demo，一个是电子商务交易，一个是仓储物流系统
### 1.2.1 流程
- 案例
    - 案例包括了有限的生命周期，对应一个工作流的开始和结束
    - 案例在某个生命周期内的某个状态，有三个元素
        - 案例变量（实例的参数）：例如 研究生GPA的成绩，GPA<2.7就不能开题。 案例相关属性的值，随案例进展而发生变化。 和流程判断有关
        - 已经满足的条件：案例状态相关的属性参数，说明案例进展
        - 案例的内容（应用数据）：和工作流程判断没有关系。 工作流系统通常不保存案例内容和细节，可能由其他系统管理
- 任务是逻辑工作单元
    - 任务不是流程实例的一次执行，而是流程中具体划分的逻辑任务的执行
    - 大概就是对任务的定义 不是说任务就可以是单独做一件事情了（不是很清楚
- 触发器
    - 四种触发图示
    - petrix网的展示，可以用触发器标识了
- 路由
    - 实现 通过路由实现控制 是工作流的核心特点
    - 四种路由的基本结构
        - 顺序路由
        - 并行路由 定义没有严格执行顺序的，可以同时进行的分支活动
        - 选择路由 多条路之间，相互制约与排斥关系的分支活动 选择时显示的，可以基于逻辑值
        - 显性或分支的选择可以预先写在路由中，这是place连接两个transaction做竞争是达不到的（后者是随机的，叫做隐性或分支）
        - 四种不同的基于Petrix网的工作流模型基本语法
        - 基于上面就有一种新的构建Petrix网的例子
# 第四章 基于业务架构的企业软件实施
- 1 企业资源管理基础
    - 1.1 企业资源管理系统ERP
        - ERP enterprise resource planning
        - 企业：从事生产、流通或服务等互动，为满足社会需要进行**自主营业、自负盈亏、承担风险、实行独立核算**，具有法人资格的基本经济单位
        - 资源：有形资源 无形资源
        - 计划：为了实现目标而拟定的具体内容和步骤
        - ERP系统主要功能：
            - SAP基础模块：SD, MM, PP, FI&CO
            - ERP三大流程：采购、生产、销售
    - **（1）生产类型**
        - 订货生产（Make To Order——MTO）
            - 根据网上客户订单来拉动，按照用户要求进行设计和组织生产，有了订单再生产，大部分产品都采用这种模式。根材料清单、并从库存系统你那个据订单要求进行专门设计和组织生产，整个过程的管理按工程管理的方法进行。生产系统根据订单情况决定生成产品生产需要的材料清单，并从库存系统取料，开展生产以得到满足用户订单的成品，放入库存，再将货物发送给用户
            - 主要产品包括专用设备、软件定制
        - 备货生产（Make To Stock——MTS）
            - 根据以往的生产情况和市场情况进行预测，按照已有的标准产品或者标准产品系列进行生产，如包括家用电器、日常生活用品等。生产按补充库存为目的进行组织，通过成品库存满足用户的不确定需求。产品需求一般比较稳定而且可以预见，产品规格及种类较少，产品允许保留较长时间，产品存储在仓库中，根据需要最是提取，生产计划的主动权较大。
            - 家用电器、日常生活用品、药品
        - 订货组装（Assemble To Order——ATO）
            - 部件预先生产加工，储存在中间库房，在客户对零部件或者产品的某些配置给出要求，生产商根据客户的要求提供为客户定制的产品。生产以模块化设计为前提，必须备有不同部件并准备好多个柔性的组装车间，以便在最短期内组装出种类众多的产品。交货期短
            - 如计算机和工作站，办公家具、房屋门窗以及某些机械产品。
        - 工程生产（Engineer To Order——ETO）
            - 与MTO的多系列品种小批量生产相比，ETO更多的是单件复杂生产过程，生产周期长、过程复杂、涉及人员多。也被称为转向生产。市场需求允许在一段时间后交货，生产和存储费用较大，可以减少产品库存量甚至实现“零库存”
            - 如重装备，船舶，飞机等
    - 不同的生产类型，生产拉动的方式完全不同，甙类计划模式差别很大。生产类型是需求制定的首先考虑问题
    - （2）物料编码
        - 物料编码有时也叫做物料清单，计算机系统对无聊的**唯一**识别代码
        - 每种物料必须有对应且唯一的物料编码
        - 设计编码体系要科学合理
        - 按照国家、企业的规定设置
        - 一经确定不能轻易修改，但要有一定的扩充性
        - 便于使用和记忆
        - 编码是管理思想的体现，管理在前，分类在后
    - （3）物料清单
        - BOM表单
        - 基本型BOM
        - 计划型BOM
        - 模块型BOM
        - 成本型BOM
        - 要保证BOM的准确性在98%以上，成本控制，信息管理的核心
    - （4）设备
        - 工作中心Working Center，是生产加工单元的统称，在完成一项加工任务的同时也发生了加工成本。它室友一台或几台功能相同的设备，一个或多个工作人员，一个小组
        - 关键工作中心，也成为瓶颈工程，bottleneck，是运行粗能力计划的计算对象
        - 特点：
            - 进城满负荷，加班加点工作
            - 需要技术熟练工人操作，不能任意替代
            - 工艺独特的专用设备，不能代替或者分包外协
            - 价格昂贵的设备，不能随时增加
            - 受多种限制，如短期内不能随便增加负荷和产量（受场地、成本等约束）
    - （5）工艺路线
        - 物料实际加工和装配的工序顺序、工序使用的工作中心，各项时间定额等等。
        - 工艺路线也就是加工的流程
        - 工艺路线的作用
            - 用于MPR计划和能力计划的生成与平衡
            - 计算物料提前期
            - 生成车间生产作业计划
            - 物料成本核算
            - 跟踪控制产品的生产
            - 专门用作工艺路线应用的CAPP系统
    - （6）提前期与计划展望期
        - 生产加工（或装配）提前提：
            - 构成：排队、准备、加工、等待和传送
        - 固定提前期：与加工数量无关，常用与物料采购
        - 变动提前期：与加工数量有关，常用与物料加工
        - 生产提前期 = 排队时间 + 准备时间 + 批量 x 单位加工时间 + 等待时间 + 传送时间
        - 其中的排队时间、等待时间和传送时间又被称为保险期或者缓冲期
    - （7）独立需求和相关需求
        - 独立需求由MPS下达，用过预测或用户订单得到
        - 相关需求是通过物料需求计划运算后得到
# hw3 - BPMN
- 4.1 业务流程管理
- 业务流程建模标注（Business Process Modeling Notation），目标是提供一些容易被业务用户理解的一套描述语言，提供业务分析者、软件开发者以及业务管理者和监察者使用
- BPMN定义了一个业务流程图，该流程图被设计用于创建业务流程操作的图形化模型
# 12/17
- 排队论
    - 随机服务系统理论 适用于系统的等待时间、完成时间和资源利用率等性能指标进行分析
    - xxx没记到
    - 排队规则
        - 等待制
            - 先到先服务
            - 后到先服务
    - 排队系统的kendall表示
        - A/S/m/B/K/SD
        - A:表示顾客相继到达时间间隔的分布概率
            - M
            - D
            - Ek
            - G
        - S:表示服务时间分布，所用符号与A一样
        - m:表示服务台个数，取正整数。1表示单个服务台，m表示多个服务台
        - B:表示系统中顾客容量限额
        - K:便是顾客源限制，可以取正整数或无穷，即有限或者无限两种
        - SD:表示服务规则，如FCFS,LCFS等
    - 对于一个流程，主要性能指标：
        - 平均WIP（队列长度）
        - 案例完成时间（平均流动时间，等待时间）
        - 资源利用率（工作负荷，关键设备占用情况）
