
## SNA-FGD(Family Group Detection in Social Network Analysis)<br>

> 参考：[SNA相关会议期刊列表](https://github.com/Tulongf/awesome-CA/blob/master/jclist.md)<br>
搜索关键词：`Community detection` `Detecting family`  `relationship labeling`

##1.若干会议的期刊论文梳理
###1.1 [ICWSM: The International AAAI Conference on Web and Social Media](http://icwsm.org/2017/index.php)
#### 2016 topic相关梳理
* 个人特征模型<br>
  * `年龄预测`<br>
Zhang J, Hu X, Zhang Y, et al. Your Age Is No Secret: Inferring Microbloggers’ Ages via Content and Interaction Analysis[C]//Tenth International AAAI Conference on Web and Social Media. 2016.<br>
  * `给朋友关系标签`<br>
 Park J Y, Sohn Y, Moon S. Power of Earned Advertising on Social Network Services: A Case Study of Friend Tagging on Facebook[C]//Tenth International AAAI Conference on Web and Social Media. 2016.<br>
  * `理解仇恨讨厌的情绪`<br>Silva L, Mondal M, Correa D, et al. Analyzing the Targets of Hate in Online Social Media[J]. arXiv preprint arXiv:1603.07709, 2016.<br>
  * `根据用户使用的APP对用户进行画像`<br>Malmi E, Weber I. You Are What Apps You Use: Demographic Prediction Based on User's Apps[J]. arXiv preprint arXiv:1603.00059, 2016.<br>
  * `根据twitter的数据定位家庭位置和活动位置`<br>Hossain N, Hu T, Feizi R, et al. Precise Localization of Homes and Activities: Detecting Drinking-While-Tweeting Patterns in Communities[C]//Tenth International AAAI Conference on Web and Social Media. 2016.<br>
  * `理解仇恨讨厌的情绪`<br>Jones I, Wang R, Han J, et al. Community Cores: Removing Size Bias from Community Detection[J]. 2015.<br>

* 社交推荐<br>
Celis L E, Krafft P M, Kobe N. Sequential Voting Promotes Collective Discovery in Social Recommendation Systems[J]. arXiv preprint arXiv:1603.04466, 2016.

* 群体推荐<br>
Pramanik S, Gundapuneni M, Pathak S, et al. Predicting Group Success in Meetup[C]//Tenth International AAAI Conference on Web and Social Media. 2016.

* 计算广告<br>
  * `根据twitter的数据预测用户兴趣，如果给定一个广告、那么会分析出一个最佳的线下广告投放的区域`<br>Anagnostopoulos A, Petroni F, Sorella M. Targeted Interest-Driven Advertising in Cities Using Twitter[C]//Tenth International AAAI Conference on Web and Social Media. 2016.<br>
  * `facebook，设备跨屏打通`<br>Coey D, Bailey M. People and Cookies: Imperfect Treatment Assignment in Online Experiments[C]//Proceedings of the 25th International Conference on World Wide Web. International World Wide Web Conferences Steering Committee, 2016: 1103-1111.

#### 2015 topic相关梳理
* `挖掘隐含的用户特征`<br>Chen J, Haber E, Kang R, et al. Making use of derived personality: The case of social media ad targeting[C]//Proceedings of the International AAAI Conference on Web and Social Media (ICWSM). 2015.<br>
* `分析用户在现实与网络中的活动参与`<br>Hu Y, Farnham S, Talamadupula K. Predicting user engagement on twitter with real-world events[C]//Proceedings of the International Conference on Weblogs and Social Media (ICWSM). AAAI. 2015.<br>
* `根据照片分析家庭位置和旅游位置`<br>Zheng D, Hu T, You Q, et al. Towards lifestyle understanding: Predicting home and vacation locations from user’s online photo collections[C]//Proceedings of the 9th International AAAI Conference on Web and Social Media. 2015: 553-560.
* `分析隐私行为`<br>Dong C, Jin H, Knijnenburg B P. Predicting privacy behavior on online social networks[C]//Proceedings of the AAAI Conference on Web and Social Media. 2015.
* `基于位置的社交用户区分以及位置理解`<br>Rossi L, Williams M J, Stich C, et al. Privacy and the city: User identification and location semantics in location-based social networks[J]. arXiv preprint arXiv:1503.06499, 2015.
* `分析用户的互动行为`<br>Carton S, Adar E, Park S, et al. Audience analysis for competing memes in social media[C]//Ninth International AAAI Conference on Web and Social Media. 2015.
* `分析朋友间关系网络从三个方面影响着小群组团体`<br>Polonski V W, Hogan B. Assessing the Structural Correlates between Friendship Networks and Conversational Agency in Facebook Groups[C]//Ninth International AAAI Conference on Web and Social Media. 2015.

### [ASONAM: The IEEE/ACM International Conference on Advances in Social Networks Analysis and Mining](http://sbp-brims.org/2016/acceptedpapers/)
###[ISCI: International Conference on Social Computing](http://sbp-brims.org/2016/)



##2.论文list
###论文分类梳理
####(1)如何得到用户特征（数据预处理类别：侧重于处理数据集，获取数据集，处理数据成可以分析的）
####(2)用户特征建模（如何对数据建模：根据数据生成关系标签）
####(3)用户间关系挖掘、群体发现（community/group detection 方法类别）
* Wan H Y, Lin Y F, Wu Z H, et al. Discovering typed communities in mobile social networks[J]. Journal of Computer Science and Technology, 2012, 27(3): 480-491.<br><br>
> 本文个人总结：<br><br>
EI检索的文章，主要内容：<br>
  ● 数据源：利用移动运营商的通话记录、短线、手机开关机导致的基站切换日志信息<br>
  ● 数据预处理：<br>
      ○ 考虑节日与假日的区别（比如在工作日白天联系多的人是同事，那么在假日白天联系多的人更大概率是一起出去旅游家人）<br>
      ○ 需要考虑人的作息时间，这里假设人们都是在白天工作<br>
      ○ 考虑人的习惯，有的人用打电话频率低、那么打了电话说明关系不一般；有的人打电话的时间习惯也不一样，需要归一化处理这些互动，以得到一致性的互动强度的表示<br>
  ● 打用户间关系标签：利用家庭团体、公司同事团体之间在上下班期间的互动程度来对用户之间的关系打标签（比如用户1和用户2是家人之类）<br><br>
      ○ 其他方法回顾：directed models (such as Bayesian networks) and undirected models (such as Markov networks)<br>
      ○ 特征建立，具体就是归一化度量打电话、发短信、位置这些特征；<br>
          ■ 可以根据基本属性，例如年龄、性别、教育、兴趣等划分小团体，当然这也可以作为对隐含关系的推断方法。社交关系与画像的打通，可以打通画像系统与六脉的感觉、根据画像推断关系、反过来可以验证关系挖掘的正确性；<br><br>
      ○ 难点：处理依赖关系，U1和U2是家人、U2和U3是家人，那么U1和U3是不是家人？<br>
      ○ CRF算法打标签<br>
          ■ 简单理解：我认识超哥P（t/w），超哥认识亮哥P(w/z)、我自己也认识亮哥P(t/z)，那么如何计算我与亮哥的关系, P(t/z) =? P(t/w)*P(w/z)+P'(t/z)<br>
          ■ 参考文章：http://blog.csdn.net/discxuwei/article/details/6331617
  ● 根据关系标签划分团体：根据用户间关系的标签图模型，来划分社区（难点是考虑标签之间的依赖关系，比如A和B是家人、B和C是家人，那么A和C也应该是家人，等等）<br>
      ○ 回顾了一下其他方法：modularity-based algorithms, Spectral algorithms, methods based on statistical inference, label propagation algorithm (LPA)；文献【19】是一篇综述<br>
      ○ 本文方法：<br>
          ■ 方法一：根据关系强度去掉弱标签，比如A和B是家人，那么去掉相关的同事关系标签，就会得到一个家庭小团队；<br>
          ■ 方法二：根据概率模型，决定哪些关系标签应该去掉、使得去掉标签之后的形成的两个团体之间的用户关系更密切；Infomap algorithm进行团体发现、文献【22】。这说明把一个人强行划到一个团体（例如家庭）的做法不一定合理，如果已经有的数据显示他和另外一个小团体（比如同事团体）的联系更紧密、相似度更高的话，那么最合理的划分是将其划到最大相似度的那个团体，而不是非要明确的标记那个团体是什么；<br>
  ● 如何评价一个小团体划分是否合理<br>
      ○ 其他方法：参考【24】、【25】<br>
      ○ 作者的方法：计算群体两个用户被准确划分到一个团体的整体准确率。简单理解就是，如果U1、U2是实际属于一个团体的，那么U1、U2的计算结果如果属于一个团体那么标记为一次正确的划分、否则标记为失败分类，统计系统正确划分的占比作为评价指标。<br>
      
####(4)应用优化、如何利用已经得到的结论优化某个场景的应用
####(5)评价指标一类

###未整理列表
