# 无障碍电影旁白标注-任务指导

## 任务背景
无障碍电影，就是在普通电影中加入实时描述画面内容的旁白，便于视力障碍者观看。我们希望能从现有的无障碍电影中提取出旁白内容，但利用AI语音转文字的效果不够好，需要在此基础上进行一些人为的校正。信息学院AIM3实验室正在招募一些志愿者一起完成校正工作，有兴趣参与的可以扫码加群了解详情~

## 任务说明
观看西瓜视频上的无障碍版电影，修正电影旁白word文件。具体工作包括删去掺杂在旁白里的演员台词、修改错误的旁白句子等等。修改完毕后，将无错误的纯旁白（不含电影人物台词）word文件发给工作人员检查确认即可。**每部电影时长约 2 小时，观看电影并完成一部电影旁白的修正工作共耗时约 3 小时，酬劳为 50 RMB/部。**  
参与任务的小伙伴需要依次完成下面这些工作：  

### 1. 电影片段试标
- 为了帮助大家熟悉工作、避免一些常见的问题，我们设计了一个小片段给大家试标。点击[【试标片段】](files/%E3%80%8A%E6%88%91%E4%B8%8D%E6%98%AF%E8%8D%AF%E7%A5%9E%E3%80%8B%E8%AF%95%E6%A0%87%E6%97%81%E7%99%BD.docx)下载试标片段和旁白初稿，请根据电影片段对初稿进行修正。
- 将修正后的旁白稿发给工作人员，工作人员会根据各位的试标效果给出建议。  

### 2. 任务认领
- 点击[【在线表格】](https://docs.qq.com/sheet/DS1ljaEZEY3Nxb29u?tab=BB08J2)可以查看电影列表，小伙伴们可以认领自己感兴趣的电影，并在备注中填入自己的名字表示该电影已认领。（已经有人认领的电影不可以重复认领，否则不计入有效工作哦）  
- 认领完成后，可以在[页面底端](#文件下载)获取相应电影的旁白初稿（点击电影名即可下载）和在线观看地址。

### 3. 电影标注
- 从本页面下载的旁白初稿是一个word文件，请尽量不要修改文件名。打开该文件，选择UTF-8编码格式（若文件可自动正常打开，此步省略）。

<div align=center>
<img src="images/0.jpg" width="50%" alt=""/>
</div>

- 打开上述在线表格中的电影在线观看地址，一边观看电影，一边修正word文件中的旁白，可以采用分屏或者多设备等方式。

<div align=center>
<img src="images/1.jpg" width="75%" alt=""/>
</div>

- 修改内容主要包括两部分：**修正错误的旁白**和**删去非旁白的电影台词**。可能出现的待修正情况请见[标注细节](#标注细节)。

### 4. 成果提交
- 修正完成后，直接将word文件发给工作人员，等待质检，确认无误，则标注完毕。  
- 若有兴趣，可继续认领其它任务，直到所有任务全部被认领为止。

## 标注细节
本次标注目标为获得干净无误的电影旁白文件。因此需要标注者对当前的旁白文件进行清洗与错误修正。可能存在的需修改的情况罗列如下（包括但不限于）：

**1. 删去演员台词和讲述人翻译演员台词的相关文本，仅保留电影旁白。**  
当前的旁白文件中混杂了一些演员台词或英文台词的中文翻译，请将这部分内容删去。如整条句子均为台词或无意义的语句，则将整条数据连同时间戳一起删掉。  
> **示例1：内容为旁白与台词的混杂**  
> 修改前：`0:58:6-0:58:15` ~~来了大家加油，再接再厉，乘~~**5人组**在店里吃起了火锅，~~啊我给你们大家讲的事情，~~  
> 修改后：`0:58:6-0:58:15` 程勇五人坐在店里吃起了火锅。    
> 修改原因：划线部分是演员台词，应该删除；加粗部分为错误的旁白，应该修改。

> **示例2：内容包含外语台词翻译**  
> 修改前：`0:5:17-0:5:24` 泰勒深呼一口气回答了声，~~好~~，戴帽子的工作人员转头说，~~各就各位，我们再来一次，~~  
> 修改后：`0:5:17-0:5:24` 泰勒深呼一口气回答了声，戴帽子的工作人员转头说。  
> 修改原因：划线部分为讲述人翻译英文台词，并非讲解的旁白，应该删掉。

> **示例3：整条内容全部为台词或其他非旁白内容**  
> 修改前：`0:7:24-0:7:31` 唉呀马晶你干嘛呀吓死我了，你神经病啊什么？呢你一听一让你来飞过去，  
> 修改后：  
> 修改原因：由于整条句子全为台词或其他非旁白内容，因此将此条数据连同时间戳一起删掉。  

**2. 修改旁白中错误的人名，包括演员名，工作人员名以及角色名等。**
> **示例1：**  
> 修改前：`0:0:24-0:0:37` 今天要为您讲述的电影是西红柿首富，该片由闫**飞**、彭大魔编剧**间**指导，由沈腾、宋**云华**、张一鸣、常远、张晨光、魏翔等主演。  
> 修改后： `0:0:24-0:0:37` 今天要为您讲述的电影是西红柿首富，该片由闫非、彭大魔编剧兼指导，由沈腾、宋芸桦、张一鸣、常远、张晨光、魏翔等主演。  
> 修改原因：本例中，编剧和演员名都有错误，应该修改。另外，本例还存在一个错别字“间”，应修改为“兼”。  

> **示例2：**  
> 修改前： `0:0:59-0:1:16` 但是王老太爷给出了一个非常奇葩的条件，那就是要求王多鱼在一个月内花光 10 亿，还不能告诉身边的人，否则就会失去继承权，王多鱼毫不犹豫**的**签下军令状，随后与好友**装强**以及财务**下竹**一起开启了**灰金之旅**。  
> 修改后： `0:0:59-0:1:16` 但是王老太爷给出了一个非常奇葩的条件，那就是要求王多鱼在一个月内花光 10 亿，还不能告诉身边的人，否则就会失去继承权，王多鱼毫不犹豫地签下军令状，随后与好友庄强以及财务夏竹一起开启了挥金之旅。  
> 修改原因：本例中，加粗的演员角色名有错误，应该修改。另外，本例还存在错别字“的”、“灰”，应分别修改为“地”、“挥”。

**3. 修改旁白中的错别字**
> 示例：  
> 修改前： `0:1:32-0:1:45` 该片于 2018 年 7 月 5 号在中国上映，本片部分内容取于真实事件，但人物情节均为虚构，剧作属于**在**创作，并非真实记录。  
> 修改后： `0:1:32-0:1:45` 该片于 2018 年 7 月 5 号在中国上映，本片部分内容取于真实事件，但人物情节均为虚构，剧作属于再创作，并非真实记录

**4. 若文本出现断句错误，标点符号错误，请根据语言习惯进行修正。**
> 示例：  
> 修改前： `0:2:35-0:3:0` 影片开头程勇一个人坐在保健品店里，程勇没有理会电话铃声吸了一口烟接着玩蜘蛛纸牌，画面转到程勇店门口，店面坐落在破旧的小巷里，隔壁情缘宾馆的老板这时候出来到程勇店里**老常老常**  
> 修改后：`0:2:35-0:3:0` 影片开头`，`程勇一个人坐在保健品店里，程勇没有理会电话铃声`，`吸了一口烟，接着玩蜘蛛纸牌`。`画面转到程勇店门口，店面坐落在破旧的小巷里，隔壁情缘宾馆的老板这时候出来到程勇店里`。`  
> 修改原因：本例修改前的旁白有多处标点符号错误或遗漏，导致阅读不顺畅。应进行一些标点符号的增添或修改，如高亮部分。加粗的文字为演员台词，应该删去。

**5. 如果发现有旁边缺失，无需手动输入补回。** 考虑到人工增加遗漏旁白的工作量较大，我们不硬性要求标注者将缺失的大段旁白补回。  

PS：也可以[【点击此处】](files/%E4%BB%BB%E5%8A%A1%E8%AF%B4%E6%98%8E.pdf)查看或下载PDF版任务说明。

## 文件下载

|序号|电影名（点击下载旁白）|在线观看地址|
| ---- | ---- | ---- |
|1|[七月与安生](files/7012955608462983717.doc)|[在线观看](https://www.ixigua.com/7012955608462983717)|
|2|[101次求婚](files/7010672852361806350.doc)|[在线观看](https://www.ixigua.com/7010672852361806350)|
|3|[狄仁杰之通天帝国](files/6997701458141381150.doc)|[在线观看](https://www.ixigua.com/6997701458141381150)|
|4|[天将雄师](files/7042487509435040292.doc)|[在线观看](https://www.ixigua.com/7042487509435040292)|
|5|[太极1 从零开始](files/7045997377349485063.doc)|[在线观看](https://www.ixigua.com/7045997377349485063)|
|6|[幕后玩家](files/7025764136805990920.doc)|[在线观看](https://www.ixigua.com/7025764136805990920)|
|7|[唐山大地震](files/6973234995351519752.doc)|[在线观看](https://www.ixigua.com/6973234995351519752)|
|8|[分手合约](files/7042578177918665252.doc)|[在线观看](https://www.ixigua.com/7042578177918665252)|
|9|[快把我哥带走](files/7028738936197349896.doc)|[在线观看](https://www.ixigua.com/7028738936197349896)|
|10|[线人](files/7037862296051253796.doc)|[在线观看](https://www.ixigua.com/7037862296051253796)|
|11|[消失的子弹](files/7021806173343089160.doc)|[在线观看](https://www.ixigua.com/7021806173343089160)|
|12|[何以笙箫默](files/7014119425527775780.doc)|[在线观看](https://www.ixigua.com/7014119425527775780)|
|13|[风声](files/6973464009504719373.doc)|[在线观看](https://www.ixigua.com/6973464009504719373)|
|14|[超级保镖](files/7053351599829156359.doc)|[在线观看](https://www.ixigua.com/7053351599829156359)|
|15|[嫌疑人X的献身](files/7008455741547741732.doc)|[在线观看](https://www.ixigua.com/7008455741547741732)|
|16|[全城热恋](files/6975440804718313992.doc)|[在线观看](https://www.ixigua.com/6975440804718313992)|
|17|[从你的全世界路过](files/6965779415842161159.doc)|[在线观看](https://www.ixigua.com/6965779415842161159)|
|18|[城市之光](files/7030765405027172900.doc)|[在线观看](https://www.ixigua.com/7030765405027172900)|
|19|[大鱼海棠](files/7050705736501985799.doc)|[在线观看](https://www.ixigua.com/7050705736501985799)|
|20|[私人订制](files/6989800101086495268.doc)|[在线观看](https://www.ixigua.com/6989800101086495268)|
|21|[绣春刀2 修罗战场](files/7023687019075371533.doc)|[在线观看](https://www.ixigua.com/7023687019075371533)|
|22|[春娇与志明](files/6969137574476513823.doc)|[在线观看](https://www.ixigua.com/6969137574476513823)|
|23|[妖铃铃](files/7019238835741524516.doc)|[在线观看](https://www.ixigua.com/7019238835741524516)|
|24|[狄仁杰之四大天王](files/7007736574934778382.doc)|[在线观看](https://www.ixigua.com/7007736574934778382)|
|25|[咱们结婚吧](files/6973235168161038861.doc)|[在线观看](https://www.ixigua.com/6973235168161038861)|
|26|[后来的我们](files/7004758927023800840.doc)|[在线观看](https://www.ixigua.com/7004758927023800840)|
|27|[动物世界](files/7047085811334021668.doc)|[在线观看](https://www.ixigua.com/7047085811334021668)|
|28|[危城](files/7047478908500836878.doc)|[在线观看](https://www.ixigua.com/7047478908500836878)|
|29|[魔警](files/7026973788990669342.doc)|[在线观看](https://www.ixigua.com/7026973788990669342)|
|30|[羞羞的铁拳](files/6979403183571337742.doc)|[在线观看](https://www.ixigua.com/6979403183571337742)|
|31|[追龙](files/6973286990817002015.doc)|[在线观看](https://www.ixigua.com/6973286990817002015)|
|32|[夜宴](files/7054867550626120205.doc)|[在线观看](https://www.ixigua.com/7054867550626120205)|
|33|[前任3 再见前任](files/6977702276018536996.doc)|[在线观看](https://www.ixigua.com/6977702276018536996)|
|34|[每当变幻时](files/7037091402852860423.doc)|[在线观看](https://www.ixigua.com/7037091402852860423)|
|35|[黄金兄弟](files/7028941404327903774.doc)|[在线观看](https://www.ixigua.com/7028941404327903774)|
|36|[美人鱼](files/6965779678749524488.doc)|[在线观看](https://www.ixigua.com/6965779678749524488)|
|37|[八卦宗师](files/7031490154833379870.doc)|[在线观看](https://www.ixigua.com/7031490154833379870)|
|38|[大腕](files/6977652368879911454.doc)|[在线观看](https://www.ixigua.com/6977652368879911454)|
|39|[血狼犬](files/7046773901736706573.doc)|[在线观看](https://www.ixigua.com/7046773901736706573)|
|40|[即日启程](files/7034019758806663710.doc)|[在线观看](https://www.ixigua.com/7034019758806663710)|
|41|[二十二](files/7021829520667705869.doc)|[在线观看](https://www.ixigua.com/7021829520667705869)|
|42|[解忧杂货店](files/7003667578891534878.doc)|[在线观看](https://www.ixigua.com/7003667578891534878)|
|43|[记忆大师](files/6992521335159292452.doc)|[在线观看](https://www.ixigua.com/6992521335159292452)|
|44|[手机](files/6973235282313380383.doc)|[在线观看](https://www.ixigua.com/6973235282313380383)|
|45|[我家有一只河东狮](files/6978299050923655693.doc)|[在线观看](https://www.ixigua.com/6978299050923655693)|
|46|[夏洛特烦恼](files/6965768652251628068.doc)|[在线观看](https://www.ixigua.com/6965768652251628068)|
|47|[叶问3](files/7010773660500034078.doc)|[在线观看](https://www.ixigua.com/7010773660500034078)|
|48|[非凡任务](files/7021812146715492901.doc)|[在线观看](https://www.ixigua.com/7021812146715492901)|
|49|[我是证人](files/7010686199291445773.doc)|[在线观看](https://www.ixigua.com/7010686199291445773)|
|50|[武侠](files/7009164747627037220.doc)|[在线观看](https://www.ixigua.com/7009164747627037220)|
|51|[新少林寺](files/6979403047063847432.doc)|[在线观看](https://www.ixigua.com/6979403047063847432)|
|52|[赤道](files/6969128872847770149.doc)|[在线观看](https://www.ixigua.com/6969128872847770149)|
|53|[睡在我上铺的兄弟](files/7026740701350560264.doc)|[在线观看](https://www.ixigua.com/7026740701350560264)|
|54|[寻龙诀](files/6966781600558219784.doc)|[在线观看](https://www.ixigua.com/6966781600558219784)|
|55|[刺客聂隐娘](files/7047079643362361886.doc)|[在线观看](https://www.ixigua.com/7047079643362361886)|
|56|[轩辕大帝](files/7050102817800847902.doc)|[在线观看](https://www.ixigua.com/7050102817800847902)|
|57|[集结号](files/6964237627511800350.doc)|[在线观看](https://www.ixigua.com/6964237627511800350)|
|58|[建军大业](files/7027034597812601381.doc)|[在线观看](https://www.ixigua.com/7027034597812601381)|
|59|[捉妖记](files/6969009002155868709.doc)|[在线观看](https://www.ixigua.com/6969009002155868709)|
|60|[南极之恋](files/7019305834282746382.doc)|[在线观看](https://www.ixigua.com/7019305834282746382)|
|61|[无问西东](files/6992608316731949576.doc)|[在线观看](https://www.ixigua.com/6992608316731949576)|
|62|[拆弹专家](files/7002505966260322852.doc)|[在线观看](https://www.ixigua.com/7002505966260322852)|
|63|[我想和你好好的](files/7025839417755435527.doc)|[在线观看](https://www.ixigua.com/7025839417755435527)|
|64|[绝世高手](files/7045651667617841695.doc)|[在线观看](https://www.ixigua.com/7045651667617841695)|
|65|[遍地狼烟](files/6978035501643072031.doc)|[在线观看](https://www.ixigua.com/6978035501643072031)|
|66|[悲伤逆流成河](files/7019264414255677989.doc)|[在线观看](https://www.ixigua.com/7019264414255677989)|
|67|[十二生肖](files/6966492004553490981.doc)|[在线观看](https://www.ixigua.com/6966492004553490981)|
|68|[二代妖精之今生有幸](files/7022202598925173261.doc)|[在线观看](https://www.ixigua.com/7022202598925173261)|
|69|[一出好戏](files/6963963173992923684.doc)|[在线观看](https://www.ixigua.com/6963963173992923684)|
|70|[杀破狼贪狼](files/6972811453581492766.doc)|[在线观看](https://www.ixigua.com/6972811453581492766)|
|71|[李茶的姑妈](files/7041192569392333342.doc)|[在线观看](https://www.ixigua.com/7041192569392333342)|
|72|[最美的时候遇见你](files/7022527427654255134.doc)|[在线观看](https://www.ixigua.com/7022527427654255134)|
|73|[缝纫机乐队](files/6976547448567431717.doc)|[在线观看](https://www.ixigua.com/6976547448567431717)|
|74|[宫锁沉香](files/7041192186846642695.doc)|[在线观看](https://www.ixigua.com/7041192186846642695)|
|75|[全能囧爸](files/6969008770273772040.doc)|[在线观看](https://www.ixigua.com/6969008770273772040)|
|76|[妖猫传](files/7025625776515088932.doc)|[在线观看](https://www.ixigua.com/7025625776515088932)|
|77|[非诚勿扰2](files/7013684159067456037.doc)|[在线观看](https://www.ixigua.com/7013684159067456037)|
|78|[孔子](files/7031493608263909925.doc)|[在线观看](https://www.ixigua.com/7031493608263909925)|
|79|[使徒行者](files/6967326539511759368.doc)|[在线观看](https://www.ixigua.com/6967326539511759368)|
|80|[捉妖记2](files/7011023396339188232.doc)|[在线观看](https://www.ixigua.com/7011023396339188232)|
|81|[长城](files/6967326939417838110.doc)|[在线观看](https://www.ixigua.com/6967326939417838110)|
|82|[滚蛋吧 肿瘤君](files/6989800362345660936.doc)|[在线观看](https://www.ixigua.com/6989800362345660936)|
|83|[一念天堂](files/7052960987330118151.doc)|[在线观看](https://www.ixigua.com/7052960987330118151)|
|84|[恶棍天使](files/6973191792690725412.doc)|[在线观看](https://www.ixigua.com/6973191792690725412)|
|85|[太极2 英雄崛起](files/7027476439662330399.doc)|[在线观看](https://www.ixigua.com/7027476439662330399)|
|86|[非诚勿扰](files/6964710089806578190.doc)|[在线观看](https://www.ixigua.com/6964710089806578190)|
|87|[可可西里](files/7031481549027705375.doc)|[在线观看](https://www.ixigua.com/7031481549027705375)|
|88|[过年好](files/7042313900221694500.doc)|[在线观看](https://www.ixigua.com/7042313900221694500)|
|89|[连环局](files/7051542450405704222.doc)|[在线观看](https://www.ixigua.com/7051542450405704222)|
|90|[游戏规则](files/7021874945990853151.doc)|[在线观看](https://www.ixigua.com/7021874945990853151)|
|91|[侠盗联盟](files/7026623602615452196.doc)|[在线观看](https://www.ixigua.com/7026623602615452196)|
|92|[追凶者也](files/6965784412118057509.doc)|[在线观看](https://www.ixigua.com/6965784412118057509)|
|93|[邪不压正](files/6973231937657766437.doc)|[在线观看](https://www.ixigua.com/6973231937657766437)|
|94|[心花路放](files/6971682573294666247.doc)|[在线观看](https://www.ixigua.com/6971682573294666247)|
|95|[西游记之大圣归来](files/7039603537449320996.doc)|[在线观看](https://www.ixigua.com/7039603537449320996)|
|96|[影](files/6979402871376871949.doc)|[在线观看](https://www.ixigua.com/6979402871376871949)|
|97|[边境风云](files/6967711402819584543.doc)|[在线观看](https://www.ixigua.com/6967711402819584543)|
|98|[乘风破浪](files/6969128384144081416.doc)|[在线观看](https://www.ixigua.com/6969128384144081416)|
|99|[解救吾先生](files/6991751088659497479.doc)|[在线观看](https://www.ixigua.com/6991751088659497479)|
