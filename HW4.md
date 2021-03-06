## HW４
#### 1.简答题
##### 1.用例的概念
>用例是文本形式的情节描述，用以说明参与者（actor）使用某系统以实现某些目标，每个用例提供一个或多个场景，该场景（用例实例）说明了系统如何与参与者互动。 用例不是图形，是文本。
##### 2.用例和场景的关系？什么是主场景或 happy path？
>场景又称为用例实例（use case instance），是使用系统的一个特定情节 或用例的一条执行路径；用例就是一组相关的成功和失败场景的集合，场景是用 例的子集。
>主场景也被称为“理想路径”或“典型流程”，它描述了满足涉众关注点的典型成功路径。通常主场景要保持一定连贯性并将所有条件处理都推延至拓展部分。
##### 3.用例有哪些形式？
>摘要:简洁的一段式概要，通常用于主场景
>非正式：非正式的段落格式用几个段落覆盖不同的场景
>详述：详细编写所有步骤及各种变化
##### ４.对于复杂业务，为什么编制完整用例非常难？
>对于复杂的业务，需求难以把控，系统复杂庞大且可能涉及多个子系统，参与对象多样，要讨论该系统的完整用例和场景将非常困难且成本较高。
##### 5.什么是用例图？
>用例图是一种系统语境图(context diagram)，用例图能够展示系统边界、位于边界之外的事物以及系统如何被使用。用例图可以作为沟通的工具，用以概括 系统及其参与者的行为。
##### 6.用例图的基本符号与元素？
>用例图包括参与者(Actor)、用例(Use case)、关联关系(Association)、包含关系（Include）、拓展关系(Extend)和泛化关系(Generalization)
##### 7.用例图的画法与步骤
* 确定用例、系统
* 识别参与者
* 识别参与者和用例间的关系
* 作图

##### 8.用例图给利益相关人与开发者的价值有哪些？
> 软件开发时无论使用面向对象方法还是其他方法都一定要明确需求，分析典型用例是开发者准确、迅速的了解用户要求最常用、最有效的办法，用例重视文本， 用例图更直观简洁，可以方便开发者与利益相关人一起剖析系统的功能和需求。

#### 2.建模联系题
##### 选择2-3个你熟悉的类似业务的在线服务系统（或移动 APP），如定旅馆（携程、去哪儿等）、定电影票、背单词APP等，分别绘制它们用例图。
![](photo/1.png)
![](photo/2.png)

##### 1.为什么相似系统的用例图是相似的？
>相似系统面对相似的参与者和相似的需求与架构设计，其产生的场景和用例大部分都有相近之处。有些系统所依赖的子系统也是业界通用的。
##### 2.如果是定旅馆业务，请对比 Asg_RH 用例图，简述如何利用不同时代、不同地区产品的用例图，展现、突出创新业务和技术
>从业务创新的角度出发：相比于传统，当下的订旅馆扩展和创新了很多业务，如增加房型，变更提供房间的方式，这些都使得用户的选择更多，用户体验更好。
##### 3.如何利用用例图定位创新思路（业务创新、或技术创新、或商业模式创新）在系统中的作用
>依据创新用例在用例图中的关系和位置，可以很清楚的知道，创新用例依据的外部系统或者从属关系，很好的定位其服务方式和服务场景，发挥更好的服务效果。
##### 4.请使用 SCRUM 方法，选择一个用例图，编制某定旅馆开发的需求（backlog）开发计划表

| ID        |   需求名称   |   重要性   |需求目标|注意事项|
| :-------- | --------:   | :------: | :--------| :--------|
| 1         |   搜索酒店   |  90|10|可以通过关键字以及日期和城市名称进行酒店搜索|要考虑根据输入的信息进行酒店优先级排序|
| 2         |   预定酒店   |  100|15|可以查看酒店详情以及可以根据日期预定房间|要考虑房间容量以及空闲情况|
| 3         |   确认订单   |  80|8|可以修改房间以及酒店的预定信息，如时间房间号等等|要可以查看订单性情|
| 4         |   支付订单   |  70|7|可以选择不同的支付方式进行支付订单|注意支付异常反馈|

##### 5.根据任务4，参考 使用用例点估算软件成本，给出项目用例点的估算

|用例        |事务      |计算      |原因     |UC权重  |估计    |
| :-------- | --------:| :------: |:-------|:-------|:-------|
|寻找酒店    |4         |3         |        |平均    |12      |
|预定酒店    |8         |6         |        |困难    |48      |
|支付        |3         |1         |       |简单     |3       |
|评价        |5         |4         |        |平均    |20      |
