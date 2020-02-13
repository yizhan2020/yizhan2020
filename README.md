# 「疫战2020」
<br/>
# **1、 疫战 2020 介绍**
“疫战 2020”是由用友白清杰于 2 月 1 日发起的一个关于新型冠状病毒疫情防护的开源语料库。

该语料库全部由来自志愿者完成编辑撰写。志愿者有来自北师大、北航、北邮、浙大、重大、武汉理工等高校的学生和老师，有来自上海计算所、共致开源等组织的热心人士。志愿者在很短的时间自发自愿的聚集在一起，借助网络的力量分工协作，通过众包方式完成语料库的整理。百科名医的CTO赵鑫磊先生提供了大量技术支持。

语料库的语料来源于国家权威机构发布的资料，如国务院的中国政府网发布的权威回应、中国疾病预防控制中心发布的《新型冠状病毒感染的肺炎公众防护指南》、中国医学科学院北京协和医学院的相关专家编写的《协和新型冠状病毒肺炎防护手册》、人民日报的相关问答等。

我们将国家及各个公司发布的疫情相关的工具链接附在每个结果的后面。这些工具包括国务院疫情督查、征集肺炎求助者、密切接触者测量仪、疫情实时地图、心理援助电话、防疫物资供求等。通过语料库，我们将这些工具传递给每一个人，为抗击疫情贡献力量。

疫战 2020 疫情语料库秉承开源开放的原则，我们希望社会各界都可以基于该语料库，发布疫情智能问答服务和 API。

# **2、 语料说明**
## **2.1 ****语料来源**
* 国务院的中国政府网发布的权威回应、
* 中国疾病预防控制中心发布的《新型冠状病毒感染的肺炎公众防护指南》
* 中国医学科学院北京协和医学院的相关专家编写的《协和新型冠状病毒肺炎防护手册》
* 人民日报的相关问答
* 腾讯较真
* 蒲公英医学
## **2.2 ****语料规范**
一条语料由基本问题、相似问题和答案组成。一个基本问题对应多个相似问题。

答案的格式规范：

>答案正文
>来源：机构名称+文件名称
>参考连接： [http://url](http://url)
>>祝福语
>免责声明： [http://url](http://url)

常用祝福语：

提醒：棉纱口罩、海绵口罩、活性炭口罩无防护作用,请使用医用口罩

提醒：医用口罩够用，N95口罩请留给医务人员

提醒：不出门、不聚集，安全第一

提醒：不隐瞒，早发现，早治疗，早健康

提醒：勤洗手、戴口罩、不聚集、少出门、频消毒、慎揉眼、多通风

岂曰无衣、与子同袍、王于兴师，修我戈矛

众志成城，万众一心，武汉加油，中国加油

# **3、 规范**
## 3.1 资料搜集规范
## 3.2 整理规范
1、 基本问题和答案在同一行；注明【来源】和【参考链接】，来源包括来源机构+文档名词，如下图所示：

  ![图片](https://uploader.shimo.im/f/wu1Y4NqH7oswBzj9.PNG!thumbnail)

  

2、考虑大众（非医疗工作者）能够看懂答案，若字数过多可适当缩减。

3、和安全防护、口罩百科相关的资料，我们主要采用卫健委、疾控中心、协和医院、蒲公英医学四个机构的资料，其他机构的相关资料不再采用。

整理经验：

（1）EXCEL 单元格内换行方法：将光标定格在需要换行的地方，然后按键盘上的 Alt+Enter 回车键或直接设置为自动换行。

（2）插入完一个基本问题和答案后，可以适当空出几行方便相似问题组插入相似问题。

（3）链接可复制到浏览器中打开。

## 3.3 相似问题规范
相似问题的基本内涵：

1、相似问题是指和标准问题意思相同，但表述⽅式不同的问题。

2、相似问题是标准问题的有效补充，通过学习同⼀问题的多种不同表述⽅式，机器⼈才能理解⽤户提问。

3、相似问题越多，越能帮助机器⼈更加准确的理解⽤户提问。

4、在项⽬启动初期的语料准备阶段，每个标准问题应⾄少准备 3-5 个相似问题，如果能准备 10 个以上相似问法的话，机器⼈的理解能⼒会更有强。

 

相似问题的设置规范：

1、相似问题的设置和基本问题类似，表述要完整、明确、清晰。

2、在保证意思相同的情况下，⼀个基本问题的多个不同相似问法的表述⽅式差别要⼤，简而言之就是一句话用不同的说法来表达。

3、如果相似问题只是在连接词、语⽓词、标点或者词语顺序上有不同，那么对机器⼈理解⽤户提问的帮助就会⽐较有限，如对于“发货时间”这一问题的相似问法 “发货时间呢”或“发货时间？”都意义不大。

4、避免更换同义词、调整词语顺序、使用无实际意义的表达。例如：

    *  “……是对的”这一问题中“是对的”即无实际意义
    * “如何”与“怎么”是同义词，算法能处理
    * “如何戴口罩”和“口罩怎么戴”算法也可以解决

5、使用缩写和改写或者多种方法的组合对原有问题进行相似性问题改写。

6、根据问题答案进行改写

 

相似问题撰写举例：

例1：“发货时间”这一问题可以采取以下相似问法

    * 多久可以发货
    * 发货要多⻓时间
    * 什么时候发货

例 2：“退货如何办理”这一问题可以采取以下相似问法：

    * 退货流程
    * 想退货怎么操作
    * 我要退货

参考：

| 问题   | 相似问题   | 策略   | 问题答案   | 
|:----|:----:|:----|:----:|:----|:----:|:----|:----:|
| 疫情期间想少跑几趟医院，能一次多开点药吗？   | 疫情期间医院能多开药吗   | 缩写   | 疫情期间，支持医疗机构根据患者实际情况，合理增加单次处方用药量，减少病人到医疗机构就诊配药次数；对高血压、糖尿病等慢性病患者，经诊治医院医生评估后，支持将处方用药量放宽至 3 个月，保障参保患者长期用药需求。   | 
|     | 肺炎期间想少往医院跑，医院可不可以给我多开些药   | 同义替换   |     | 
|     | 现在这时候，医院可以给病人一次多开处方药吗   | 改写   |     | 
|     | 我生病了，但现在情况特殊，想少跑几趟医院，能不能一次给我多开些药   | 扩写，问题短的时候用   |     | 
|     | 慢性病患者医院能不能多开药   | 根据问题答案内容改写   |     | 
|     | 医生能否根据病人情况多开药   | 根据问题答案内容改写   |           | 
|     | 医疗机构有减少病人就诊次数的措施吗   | 根据问题答案内容改写   |     | 

以上策略分为两个部分：

1、针对原句子可进行同义替换和扩写，在算法上的效果不如缩写和改写带来的效果好，因而提倡缩写和改写或者多种方法的组合对原有问题进行相似性问题改写；

2、根据问题答案进行改写，可通过对不同方面进行归纳改写。

由于我们整理了同义词以及算法本身的能力，因而如下情况的书写是不提倡的：

| 问题   | 不推荐相似问题写法   | 原因   | 
|:----|:----:|:----|:----:|:----|:----:|
| 儿童如何佩戴口罩？   | 儿童怎么佩戴口罩？   | “如何”与“怎么”是同义词，算法能处理   | 
|     | 小孩怎么佩戴口罩   | 儿童与小孩是同义词算法能处理   | 
|     | 小学生怎么佩戴口罩   | 算法能解决   | 
| 怎么戴口罩？   | 如何戴口罩？   | 如何和怎么是同义词算法能解决   | 
|     | 口罩怎么戴？   | 调换词顺序，没意义    | 
|     | 怎么戴口罩是对的？   | “是对的”，没实际意义   | 

## 3.4 核对校验规范
1、检查格式是否符合规范：

    * 检查有无来源说明，如果内容来自权威机构，需要加上权威机构的名字；
    * 检查有无参考链接，如果没有参考链接，需要补充参考链接

2、检查内容是否来自权威机构。口罩以及安全防护有关的内容，需来自中国疾病控制中心、国家卫健委、协和医院、蒲公英医学等权威机构。

3、检查文字是否符合规范。检查是否有错别字，是否有标点符号错误。

检查过程中，如果发现问题，用显著的颜色标注。

如果发现多个基本问题答案相似，可找到后进行合并处理。

## 3.5 交互规范
1、开场白

[昵称], 你好~ 我是疫情小助手，可以回答新型冠状病毒相关问题，希望可以帮助你更好地抗击疫情、减少恐慌。

我的语料库由[疫战2020]提供支持，语料来源于国务院的中国政府网发布的权威回应、中国疾病预防控制中心发布的《新型冠状病毒感染的肺炎公众防护指南》、中国医学科学院北京协和医学院的相关专家编写的《协和新型冠状病毒肺炎防护手册》、人民日报的相关问答等。

我的技术实现由xx提供支持。

常用工具：

疫情督查：[http://t.cn/A6PqcbSP](http://t.cn/A6PqcbSP)

肺炎求助:http://t.cn/A6PE3Spx

密切接触者测量:http://t.cn/A6hhTd4j

定制疫情地图:http://t.cn/A6PkuSzp

心理援助电话:http://t.cn/A6PESDrT

防疫物资供求:http://t.cn/A6h7yLn5

同行查询：[http://t.cn/A6hUpX2S](http://t.cn/A6hUpX2S)

实时疫情：[http://t.cn/A6Pe7h7M](http://t.cn/A6Pe7h7M)

岂曰无衣、与子同袍、王于兴师，修我戈矛

免责声明：[http://t.cn/A6h72EGW](http://t.cn/A6h72EGW)

**2、找不到答案时的反馈**

我太难了！这个问题我还不知道...你可以试试下面的工具

常用工具： 

疫情督查：[http://t.cn/A6PqcbSP](http://t.cn/A6PqcbSP)

肺炎求助:http://t.cn/A6PE3Spx

密切接触者测量:http://t.cn/A6hhTd4j

定制疫情地图:http://t.cn/A6PkuSzp

心理援助电话:http://t.cn/A6PESDrT

防疫物资供求:http://t.cn/A6h7yLn5

同行查询：[http://t.cn/A6hUpX2S](http://t.cn/A6hUpX2S)

实时疫情：[http://t.cn/A6Pe7h7M](http://t.cn/A6Pe7h7M)

岂曰无衣、与子同袍、王于兴师，修我戈矛

免责声明：[http://t.cn/A6h72EGW](http://t.cn/A6h72EGW)

# **4、 工作流程**
![图片](https://uploader.shimo.im/f/zFoQLf4RfXsmwAip.png!thumbnail)
# **5、 使用要求**
* 需要显著说明基于“疫战 2020”语料库
* 需要反馈bad case和不能回答的问题
# **6、谁可以使用疫战2020？**
所有希望提供疫情常见问答服务的机构和个人。

# **7、感谢志愿者**
感谢为疫战 2020 做出贡献的志愿者。

1. **夏艳红**  北京师范大学的教育管理专业的学生 来自湖南衡阳。

2. **张劼** 在上海清算所工作

3. **叶志乐** 北京师范大学珠海分校的金融数学的学生 来自广东河源

4. **畅晋仪** 北京师范大学珠海分校汉语国际教育的学生 来自广东深圳

5. **朱贤颖**  北京师范大学学科教学(语文)专业的学生 来自江苏扬州

6. **杨采琳**  北京师范大学珠海分校会计学的学生   来自广东茂名

7. **王怡然**  北京师范大学珠海分校金融学专业的学生  来自河北唐山

8. **和静宇** 北京师范大学的教育技术学专业的学生 来自河北保定

9. **程刚**  北京邮电大学光电信息学院学生  来自安徽池州 在用友实习

10. **贺迪**  浙江大学的流行病与卫生统计专业的学生 来自浙江杭州

11. **何妍洁**   北京师范大学珠海分校外国语学院学生   来自广东深圳

12. **陈铭丹** 广东金融学院会计学专业的学生 来自广东汕头

13. **任爽**  北京师范大学学科教学数学的学生       来自黑龙江齐齐哈尔

14. **刘毅然** 北京航空航天大学软件工程专业的学生 来自四川攀枝花

15. **俞林杰** 浙江大学公共卫生学院的学生 来自浙江杭州

16. **张梦** 北京师范大学学科教学数学的学生 来自山西运城

17. **谢金** 武汉理工大学电子商务专业的学生  来自湖北荆州 在用友实习

18. **王钰晴**  重庆大学经济与工商管理学院学生 来自山东德州 在用友实习

19. **刘芸**  河南大学土木工程专业的学生  来自河南三门峡

20. **庄秀丽** 北京师范大学 教育学部教师

21. **陈丽娜**   长沙学院市场营销专业的学生  来自湖南郴州

22. **金歌**  ‘中国石油大学’工程管理的学生，笔记达人与幕布：共创达人。来自安徽-萧县。

23. **马纪阳**   北京师范大学珠海分校工业设计学生

24. **周游**  北京师范大学教育管理专业的学生，来自云南曲靖

25. **贺希** 湖南第一师范学院小学教育专业的学生，来自湖南长沙

26. **陈媛** 全职太太，来自北京

27. **王建华** 江西省上饶市广信区教研室 英语教研员

28. **舒坤** 武汉工商学院 教辅类老师 来自湖北武汉

29. **侯燕**  北京师范大学珠海校区 法律硕士 来自甘肃天水

30. **霍然** 北京师范大学 2019级法律硕士 来自河北保定

31. **贾苗雨田** 内蒙古师范大学新闻传播学院来自内蒙古鄂尔多斯

32. **周秋凌** 北京师范大学心理健康教育学生来自河南信阳

33. **宁青云**  北京师范大学教育硕士  来自湖南

34. **张珍**  北京师范大学教育硕士  来自湖北

35. **刘洁** 全职太太，来自天津

36. **张爽** 北京师范大学学科教学数学的学生 来自广东汕头

37. **孙阳玲** 湖南科技职业学院毕业  来自湖南长沙，目前从事健身行业

38. **孙婧雅**  河北大学旅游管理专业学生  来自河北衡水

39. **高山** 目前在职 来自河北保定

40. **周丽丽**  北京师范大学外国语言文学学院硕士  来自内蒙古呼伦贝尔

41. **蔡仁**

42. **杨赛** infoq编辑

43. **刘颂** 前用友员工 待业在家

44. **杨爽** 全职太太 来自苏州

45. **李少萍** 用友员工

46. **朱俊彬** 用友员工

47. **张蒙** 从事互联网运营工作    来自湖北武汉

48. **康小路** 北京师范大学教学管理专业学生   来自甘肃兰州

49. **陈智民**

51. **冯斯京** 宁夏大学学科教学（英语）硕士 北京邮电大学附属小学教师**

# **8、合作的伙伴**
1. 用友
2. 微信开放平台
3. 开源社
4. 爱因互动
5. 句子互动
# **9、情人节献礼**
2 月 14 日，我们联合多家机构，向社会免费提供疫情智能问答服务和 API，这是我们送给全国人民的情人节礼物。


用友旗下协同平台友空间，面向所有企业及组织提供统一数智化工作入口、协同办公、社交沟通、业务协同等核心解决方案。友空间内置智能机器人“小友”，搭载了疫情防护问答服务。用友人工智能团队基于该语料库发布了疫情智能问答API，该API发布在了用友APILink开放平台上，API免费向社会开放。

微信对话开放平台是腾讯微信AI团队打造的一款智能对话机器人配置平台，为疫情助手机器人提供了强大的自然语言处理的技术支持。同时，利用微信对话开放平台的开放能力，将疫情助手机器人相关的技能开放到了平台内技能商店中，可供所有开发者免费使用，助力其在公众号、小程序以及第三方web、app等渠道，为有需要帮助的广大群众提供更加方便的疫情查询渠道。微信AI团队秉持“以人为本，科技向善”的理念，联合所有开发者，用AI的方式，为抗击疫情作出一点绵薄贡献。


开源社基于该语料库发布疫情智能问答服务，目前已在开源社微信公众号后台提供服务，开通了和开源社疫情微信聊天机器人服务。句子互动为微信聊天机器人提供接入服务和技术支持，后台的智能对话平台，由微软（亚洲）互联网工程院的商业人工智能团队提供技术支持以及Azure云资源。


爱因互动作为第一家向项目提供对话机器人技术支持的公司，派出了产品经理和工程师给予支持。爱因互动使用志愿者建设的语料，训练智能问答机器人模型，向公众免费提供疫情知识问答机器人服务。


句子互动是一家基于微信生态，为企业提供营销销售自动化和社群管理工具的公司。配合微信对话开放平台，快速创建了疫情小助手，用户添加疫情小助手为好友后，私聊直接提问或添加进入任意群并@小助手，小助手便可回答关于疫情相关的问题，缓解用户紧张情绪。同时，句子互动也将功能集成到管理系统中，方便企业快速集成，为公众提供疫情知识问答服务。

目前我们还在进行语料的最后整理和优化。我们也希望有更多志愿者参与进来，提升语料库的质量。

