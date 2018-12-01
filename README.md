# 我的前端成长之路和对未来的探索
在本仓库里，我计划记录一些自己的过去和未来的前端成长的历程，和自己对前端的探索。

出身
---
- 网络工程，在学校时打交道最多的是交换机、路由器、服务器
- 学校是二本。在学习阶段，有过一些服务器虚拟化的实践，用8台服务器和vSphere系列软件搭建过一个跨东、南校区的实验室云平台；杂七杂八的学过浅显的java、安卓
- 真正开始学前端是大三，来自于一次学校组织的实训，但是当时的老师本身视野也比较窄，也没怎么学到东西

前端经历
---
- 和大多数同学一样参加过校招；以前也没什么资源，不认识什么在大厂的师兄，都是笔试、多轮面试
- 实习是在"同程艺龙"
- 目前就职在上海的美团点评(俗称的"新美大")

过去的成长之路分享
---
前端真正启蒙是在同程艺龙火车票部门实习的那段时间，真正的稍微的打开了视野，了解到了一些前端非"画页面"的东西

#### 实习作为引子
最关键的是认识到了几个技术上对我有很大影响的人；以前一直不懂为什么他们代码要这么写，为什么可以写的比我好，思路哪来的<br>
大家也知道，问这种问题是没有用的，没经历过、好好研究过，说再多也没用；那个时候一直维持到我去美团，我渡过了很长一段迷茫期，不知道前端该怎么学，大量的看知乎前端技术讨论、segmentfault、阮一峰、vue源代码分析，但是因为知识储备的问题，看起来有点懂，其实根本不知道如何运用、这些方案都是为了解决什么问题而存在、该怎么把这些技术和自己的业务结合在一起<br>
那个时候我就一直模仿我们组的一个大牛，他的任何代码我都看，每次分享肯定去，听不懂先听着，自己后续再去看源代码，可以说整个同程的前端除了他没有人比我更清楚他写的代码；一直看，看得多了，后来真就学到了一些东西，一直影响我到现在，我是非常感激的<br>
那个时候也顺势写了这篇文章，[自制vue组件通信插件:教你如何用mixin写插件](https://segmentfault.com/a/1190000015554464)
![示意图](https://image-static.segmentfault.com/325/626/3256260828-5b3f4175215d3_articlex)

#### 为什么离开
当初我在同程的表现也算优秀，实习时获得过部门的一次"年度优秀员工"，每天过的也比较开心。<br>
主要做了微信钱包火车票里面的英文版火车票购票系统和一个公司内的数据监控平台。业务和现在比起来根本不算繁重，基本也不加班，每次业务除了不懂的，很轻松就可以写完，闲了就看自己的东西，这个期间研究了大量WebGL、svg的东西，这个时期还写了一篇[Three.js的东西，并且这篇文章还在公司层面发表了](https://screetbloom.github.io/2017/08/03/ThreeJs/#more).<br>
![three.js](./img/three.png)
但是时间长了之后，我开始越来越觉得哪里不对，感觉自己没走到正确的路上。我自己也不知道哪个地方出了问题，最直观的感受就是技术上的提升没有质的变化，忙来忙去没有技术上的大方向；我开始担心、害怕起来。<br>
因为我知道自己不是特别有天分的人，光靠自己的自学需要及其大量的时间才能有所收获，而当时的我渴望在技术上能有大的提升，希望看一眼p7技术专家是什么样子，所以我选择了离开



校招经历
---
当时也拿到了offer，所有里面最后悔的是错失了今日头条(字节跳动)的offer，当时刚好有一个github网友帮我推荐，我获得了一次面试的机会.<br>
那是人生中第一次视频面试，什么套路也不懂，基本没做准备，特意请了半天假在房间里面试。一面是一个很年轻的人面试我，感觉和我年纪差不多，算法什么的做的很差，但是面试官说问题回答的比较深入、理解比较深入透彻，就勉强给了我二面的机会。二面问业务和技术，回答的很顺利，直接三面了，三面是一个后端主管面试，都是挑简历里面的技术点在问，但是信号很不好，面试官也没有耳机，对面电流、说话声音特别吵，我根本听不清，一再的让面试官能不能再说一遍，后期通过视频可以很明显的看到他脸上的不满，问题回答的不知道怎么样，因为很多问题题目都听不太清；最后进入了hr面，简单聊了聊简历、学校。不出意料的在第二天收到了通知，**挂了**<br>
一度抑郁了好多天，感觉既失落又沮丧<br>
<br>
接下来的面试都准备了一下，后续的都还算顺利，除了根本没投的和笔试过不了的。拿到了5-6个offer，最后因为一些原因不太想去北京，就选了稍低一些薪水的上海<br>

入职美团
---
抱着极大的期待走进来，前两个月一无所获，直到一个大佬分享，才恍然大悟，原本是自己层次太低，接触不到核心的东西。后来也开始陆续接触到了一些足以兴奋的事情，目前虽然很忙，但是也开始进入了正轨，学到了不少东西。

对前端的自己一点思考
---
- 找不到出路的时候，学好nodejs，不想学太多，就只学文件流的读写，尝试自己写工具
- 用文件的思路去看待自己和其他开发写的代码
- 将代码文件看成对象、文件流，运用node(webpack、gulp)去处理、编辑、整合代码文件
- 前端模板转译、vue模板转小程序模板
- javascript沙盒，构建一个js解释器环境

#### 1.从文件流的读写开始学习node
我真正开始意识到node的重要性就是在某一天看看到有人用gulp去读写、生成文件


#### 2.组件通信进阶








