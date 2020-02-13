# 「疫战2020」
<br/>

# 1.****疫战**** ****2020**** 介绍
“疫战 2020”是由用友白清杰于 2 月 1 日发起的一个关于新型冠状病毒疫情防护的开源语料库。

该语料库全部由来自志愿者完成编辑撰写。志愿者有来自北师大、北航、北邮、浙大、重大、武汉理工等高校的学生和老师，有来自上海计算所、共致开源等组织的热心人士。志愿者在很短的时间自发自愿的聚集在一起，借助网络的力量分工协作，通过众包方式完成语料库的整理。百科名医的CTO赵鑫磊先生提供了大量技术支持。

语料库的语料来源于国家权威机构发布的资料，如国务院的中国政府网发布的权威回应、中国疾病预防控制中心发布的《新型冠状病毒感染的肺炎公众防护指南》、中国医学科学院北京协和医学院的相关专家编写的《协和新型冠状病毒肺炎防护手册》、人民日报的相关问答等。

我们将国家及各个公司发布的疫情相关的工具链接附在每个结果的后面。这些工具包括国务院疫情督查、征集肺炎求助者、密切接触者测量仪、疫情实时地图、心理援助电话、防疫物资供求等。通过语料库，我们将这些工具传递给每一个人，为抗击疫情贡献力量。

疫战 2020 疫情语料库秉承开源开放的原则，我们希望社会各界都可以基于该语料库，发布疫情智能问答服务和 API。

# 2.语料说明
## 2.1 语料来源
* 国务院的中国政府网发布的权威回应、
* 中国疾病预防控制中心发布的《新型冠状病毒感染的肺炎公众防护指南》
* 中国医学科学院北京协和医学院的相关专家编写的《协和新型冠状病毒肺炎防护手册》
* 人民日报的相关问答
* 腾讯较真
* 蒲公英医学
## 2.2 语料规范
一条语料由基本问题、相似问题和答案组成。一个基本问题对应多个相似问题。

答案的格式规范：

>答案正文
>
>来源：机构名称+文件名称
>参考连接： [http://url](http://url)
>
>祝福语
>
>免责声明： [http://t.cn/A6h72EGW](http://url)

常用祝福语：

提醒：棉纱口罩、海绵口罩、活性炭口罩无防护作用,请使用医用口罩

提醒：医用口罩够用，N95口罩请留给医务人员

提醒：不出门、不聚集，安全第一

提醒：不隐瞒，早发现，早治疗，早健康

提醒：勤洗手、戴口罩、不聚集、少出门、频消毒、慎揉眼、多通风

岂曰无衣、与子同袍、王于兴师，修我戈矛

众志成城，万众一心，武汉加油，中国加油


# 3.规范
## 3.1 资料搜集规范
## 3.2 整理规范
1、 基本问题和答案在同一行；注明【来源】和【出处链接】，来源包括来源机构+文档名词，如下图所示：

![image](https://gitee.com/yizhan2020/yizhan2020/raw/master/scr/%E6%95%B4%E7%90%86%E8%A7%84%E8%8C%83.PNG)
  

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
|:----|:----:|:----|:----:|
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
|:----|:----:|:----|
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

疫情督查：[http://t.cn/A6PqcbSP](http://url)   

肺炎求助：[http://t.cn/A6PE3Spx](http://url)  

同行查询：[http://t.cn/A6hUpX2S](http://url)     

实时疫情：[http://t.cn/A6Pe7h7M](http://url)  

定制疫情地图：[http://t.cn/A6PkuSzp](http://url)   

心理援助电话：[http://t.cn/A6PESDrT](http://url)  

防疫物资供求：[http://t.cn/A6h7yLn5](http://url)  

密切接触者测量：[http://t.cn/A6hhTd4j](http://url)  

岂曰无衣、与子同袍、王于兴师，修我戈矛

免责声明：[http://t.cn/A6h72EGW](http://url)

2、找不到答案时的反馈

这个问题我还不知道...你可以试试下面的工具

常用工具： 

疫情督查：[http://t.cn/A6PqcbSP](http://url)   

肺炎求助：[http://t.cn/A6PE3Spx](http://url)  

同行查询：[http://t.cn/A6hUpX2S](http://url)     

实时疫情：[http://t.cn/A6Pe7h7M](http://url)  

定制疫情地图：[http://t.cn/A6PkuSzp](http://url)   

心理援助电话：[http://t.cn/A6PESDrT](http://url)  

防疫物资供求：[http://t.cn/A6h7yLn5](http://url)  

密切接触者测量：[http://t.cn/A6hhTd4j](http://url)  

岂曰无衣、与子同袍、王于兴师，修我戈矛

免责声明：[http://t.cn/A6h72EGW](http://url)

# 4.工作流程
![image](https://gitee.com/yizhan2020/yizhan2020/raw/master/scr/%E5%B7%A5%E4%BD%9C%E6%B5%81%E7%A8%8B.png)
