# web-design-learned



## 1. 万物之始



### 1.1 什么是网页
>网站是指在因特网上根据一定的规则,使用HTML等制作的用于展示特定内容相关的网页集合.
>
>网页是网站中的一"页",通常是HTML格式的文件,他要通过**浏览器**来阅读.
>
>网页是构成网站的基本元素,它通常由图片/链接/文字/音频/视频等元素组成,通常我们看到的网页常以`htm`/`html`为后缀结尾,因此俗称网页为`html`文件



### 1.2 什么是HTML

> HTML是超文本标记语言Hyper Text Markup Language,它是用来描述网页的一种语言



```html
<img src="https://dss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=3363295869,2467511306&fm=26&gp=0.jpg"/>
```



> 所谓超文本,有两层含义:
>
> 1.他可以加入图片/声音/动画/多媒体等内容即超越了普通的文本限制
>
> 2.他还可以通过一个文件跳转到另一个文件,与世界各地主机文件链接即超级链接文本



### 1.3 网页的形成

> 网页是由网页元素组成的,这些元素是利用HTML标签描述出来,然后通过浏览器解析来显示给用户的
>
> 前端人员开发代码===>浏览器解析/渲染代码===>生成最后页面





## 2. 常用浏览器

> IE/Firefox/Safari/Chrome/Opera
>
> 浏览器内核(渲染引擎):负责读取网页内容,整理讯息,计算网页的显示方式并显示页面





## 3. Web标准

> Web标准是由W3C组织和其他标准化组织制定的一系列标准的集合.



### 3.1 为什么需要Web标准

> 遵循Web标准可以让不同的开发人员写出的页面更标准外,还有以下优点:
>
> 1.让Web的发展前景更广阔的;
>
> 2.内容能被更广泛的设备访问;
>
> 3.更容易被搜寻引擎搜索;
>
> 4.降低网站流量费用;
>
> 5.使网站更易于维护;
>
> 6.提高页面浏览速度



### 3.2 Web标准的构成

> 主要包括结构(Structure)、表现(Presentation)和行为(Behavior)三个方面
>
> 结构:用于对网页元素进行整理和分类,主要是HTML;
>
> 表现:用于设置网页元素的版式,颜色,大小等外观样式,主要是CSS;
>
> 行为:是指网页模型的定义及交互的编写,主要是JavaScript
>
> **最佳体验:结构/样式/行为相分离**



![image-20201212141012064](https://raw.githubusercontent.com/zhangyutongdeyonghuming/web-design-learned/main/resources/image-20201212141012064.png).





## 4. HTML



## 4.1 基本语法概述

> 1. HTML标签是由尖括号包围的关键词,例如`<html>`
>
> 2. HTML标签通常是成对出现的,例如`<html></html>`,我们称之为双标签.
> 3. 有些特殊标签是单个出现的,例如`<br/>`,称为单标签



### 4.2 标签关系

> 标签分为两类 包含关系和并列关系



> 包含关系

```html
<head>
    <title></title>
</head>
```



> 并列关系

```html
<html>
    <head></head>
    <body></body>
</html>
```



## 5. HTML基本结构标签



### 5.1 第一个HTML页面

> 每个网页都会有一个基本的结构标签(骨架) ,页面内容也是在这些基本标签上书写

| 标签            | 定义       | 说明                                                  |
| --------------- | ---------- | ----------------------------------------------------- |
| `<html></html>`  | HTML标签   | 页面根标签                                            |
| `<head></head>`   | 文档的头部 | 在head中必须设置title                                 |
| `<title></title>` | 文档的标题 | 页面的标题                                            |
| `<body></body>`   | 文档的主体 | 元素包含文档的所有内容,页面内容基本都是放到body里面的 |



```html
<html>
<head>
    <title>我的第一个页面</title>
</head>

<body>
	Hello,World!
</body>
</html>
```



### 5.2 自动生成的三处代码

> 1. `<!DOCTYPE>` :文档类型声明,作用就是告诉浏览器采用的是`HTML5`显示网页
>
> 2. `<html lang="en">` :`en`定义为英文网页,`zh-CN`就是中文网页
> 3. `<meta charset="UTF-8">` :定义网页编码`UTF-8`防止乱码



### 5.3 HTML常用标签



#### 5.3.1 标题标签

> 为了使网页更具有语义化,我们会使用标题标签,HTML提供了六个等级的网页标题,即`<h1>`到`<h6>`



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>标题标签</title>
</head>
<body>

<h1>1级标题实例</h1>
<h2>2级标题实例</h2>
<h3>3级标题实例</h3>
<h4>4级标题实例</h4>
<h5>5级标题实例</h5>
<h6>6级标题实例</h6>

</body>
</html>
```



#### 5.3.2 段落和换行标签

> 在网页中为了使文字更有条理性,就需要将文字分段显示.`<p>`标签用于定义段落,`<br/>`可以强制进行换行

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>段落和换行标签</title>
</head>
<body>
    <p>
        新华社北京12月12日电(记者胡喆）记者从国家航天局获悉，12月12日9时54分，嫦娥五号轨道器和返回器组合体经历了约6天的环月等待，实施了第一次月地转移入射，从近圆形轨道变为近月点高度约200公里的椭圆轨道。
    </p>

    <p>
        据介绍，月地转移入射主要目的是通过月球轨道上的轨道机动，<br/>使轨道器和返回器组合体进入月地转移轨道。
    </p>

    <p>
        后续，携带月球样品的轨道器和返回器组合体将择机实施第二次月地转移入射，从而摆脱月球引力，进入月地转移轨道返回地球。
    </p>

</body>
</html>
```



#### 5.3.3 案例1:新闻

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>案例1</title>
</head>
<body>
    <h1>寒潮蓝色预警：全国多地将迎降温 局地降幅达10℃</h1>
    <h4>2020-12-12 07:17:16 来源： 中国新闻网</h4>
    <p>
        据中央气象台网站消息，<br/>中央气象台12月12日06时继续发布寒潮蓝色预警：受强冷空气影响，预计，12月12日08时至12月15日08时，西北地区东部、内蒙古中西部、华北中西部、东北地区东部、黄淮大部、江汉、江淮西部、江南中西部、西南地区东部、华南中西部等地将先后降温6～8℃，其中，陕西北部、内蒙古西部、湖南西南部、贵州东南部、广西北部等地的部分地区降温可达10℃；降温过后最低气温0℃线将南压至贵州南部至浙江西北部一线。北方地区有4～6级、阵风7～8级的偏北风，南方地区有4～5级偏北风，江河湖面阵风可达6～7级，近海海区有6～8级、阵风9级的偏北风。
    </p>

    <p>防御指南：</p>
    <p>1、人员要注意添衣保暖；在生产上做好对大风降温天气的防御准备；</p>
    <p>2、门窗、围板、棚架、临时搭建物等易被大风吹动的搭建物固紧， 妥善安置易受大风影响的室外物品；</p>
    <p>3、应到避风场所避风，通知户外作业人员注意安全；</p>
    <p>4、留意有关媒体报道大风降温的最新信息，以便采取进一步措施；</p>
    <p>5、交通、公安等部门要按照职责做好道路结冰应对准备工作。</p>
　　
</body>
</html>
```



#### 5.3.4 文本格式化标签

> 在网页中有时需要设置文字的粗体/斜体/下划线等效果

| 语义   | 标签                           | 说明                          |
| ------ | ------------------------------ | ----------------------------- |
| 加粗   | `<strong></strong>`或`<b></b>` | 推荐使用`<strong>`,语义更强烈 |
| 倾斜   | `<em></em>`或`<i></i>`         | 推荐使用`<em>`,语义更强烈     |
| 删除线 | `<del></del>`或`<s></s>`       | 推荐使用`<del>`,语义更强烈    |
| 下划线 | `<ins></ins>`或`<u></u>`       | 推荐使用`<ins>`,语义更强烈    |

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>格式化标签</title>
</head>
<body>
    我是<strong>加粗</strong>的文字
    我是<b>加粗</b>的文字

    我是<em>倾斜</em>的文字
    我是<i>倾斜</i>的文字

    我是<del>加删除线</del>的文字
    我是<s>加删除线</s>的文字

    我是<ins>加下划线</ins>的文字
    我是<u>加下划线</u>的文字

</body>
</html>
```



#### 5.3.5 盒子标签

> 语义:`<div>` `<span>`标签没有语义,表示一个盒子.都用于布局

> 特点:
>
> 1. div一行只能有一个
> 2. span是小盒子 ,每行显示多个

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>盒子</title>
</head>
<body>
    <div>我是个盒子</div>
    <div>我是另一个盒子</div>
    <span>百度</span>
    <span>搜狐</span>
    <span>阿里巴巴</span>

</body>
</html>
```



#### 5.3.6 图像标签和路径



##### 5.3.6.1 图像标签

> 在HTML中 `<img>`标签用于定义HTML页面中的图像
>
> `<img src="图像url"/>`
>
> `src`是`<img>`标签的必须属性,表示图像所在的位置,`alt`是图片显示不出来时替换的文本,`title`是悬停时的文本,`width/height/border`分别是宽度/高度/边框的样式

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>图像标签的使用</title>
</head>
<body>
    <h3>图像标签的使用</h3>
    <img src="img.jpg"/>

    <h3>其他属性</h3>
    <img src="img.jpg" alt="百度来的图片" title="鼠标悬停的标题" width="200px" height="200px" border="1px"/>
</body>
</html>
```



##### 5.3.6.2 路径

> 页面中的图片会非常多,通常我们会新建一个文件夹来存放这些图像文件,这时在查找图像就需要用"路径"的方式指定图像文件的位置
>
> 路径分为:
>
> 1. 相对路径: 图片相对于HTML页面的位置
> 2. 绝对路径: 图片在磁盘的全路径或是在网络中可以访问到的url

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>路径问题</title>
</head>
<body>
<h4>当前目录下</h4>
<img src="./img.jpg"/>

<h4>下级目录下</h4>
<img src="./images/img.jpg"/>

<h4>上级目录下</h4>
<img src="../img.jpg"/>
</body>
</html>
```



#### 5.3.7 超链接标签

> 在HTML中 `<a>`标签可以定义超链接,作用是从一个页面跳转到另一个页面.



##### 5.3.7.1 语法格式

```
<a href="" target="">文本或图像</a>
```

| 属性     | 作用                                                         |
| -------- | ------------------------------------------------------------ |
| `href`   | 用于指定目标的URL地址(required),当a标签拥有了`href`,他就具有了超链接的功能 |
| `target` | 用于指定链接页面的打开方式,其中`_self`为默认值,`_black`为在新窗口打开 |

##### 5.3.7.2 链接分类

> 1. 外部链接:例如`www.baidu.com`
> 2. 内部链接:网站内部页面之间的相互链接
> 3. 空连接:如果没有确定链接目标,可以用`#`号作为`href`值
> 4. 下载地址:如果地址里面是一个文件/包,会下载这个文件
> 5. 网页元素链接:视频/音频/图像/文本等
> 6. 锚点链接:`href`写`#某个元素的id`,即可跳到这个id的元素位置



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>a标签</title>
</head>
<body>
    <div id="top"></div>

    <h3>外部链接 _self为默认,从当前窗口打开;_blank为从新窗口打开</h3>
    <a href="https://www.baidu.com" target="_blank">百度</a>

    <h3>内部链接 打开内部的网页</h3>
    <a href="./00-HTML万物之始.html" target="_blank">万物之始</a>

    <h3>空连接</h3>
    <a href="#">官网</a>

    <h3>下载地址</h3>
    <a href="./img.zip">下载地址</a>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <br/>
    <h3>锚点链接</h3>
    <a href="#top">返回顶部</a>
</body>
</html>
```





#### 5.3.8 注释

> 作为一名开发者,不能不写注释,注释可以帮助我们快速回忆起开发当时某段代码的意义.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>注释</title>
</head>
<body>
    <!--在HTML中有些文字不想在页面中展示出来,但是又非写不可,我们可以用注释来实现-->
    <h1>注释</h1>
</body>
</html>
```



#### 5.3.9 综合案例

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>案例2</title>
</head>
<body>
<h1>圣诞节的由来</h1>
<p>圣诞节（Christmas）亦称耶稣圣诞节、主降生节，天主教亦称耶稣圣诞瞻礼。
    译名为“基督弥撒”，它源自古罗马人迎接新年的 <a target="_blank"
                              href="https://baike.baidu.com/item/%E5%86%9C%E7%A5%9E%E8%8A%82/210044">农神节</a>，与基督教本无关系。在基督教盛行罗马帝国后，教廷随波逐流地将这种民俗节日纳入基督教体系，同时以庆祝耶稣的降生。但在圣诞节这天不是耶稣的生辰，因为《圣经》未有记载耶稣具体生于哪天，同样没提到过有此种节日，是基督教吸收了古罗马神话的结果。
</p>
<p>大部分的天主教教堂都会先在12月24日的平安夜，亦即12月25日凌晨举行子夜弥撒，而一些基督教会则会举行报佳音，然后在12月25日庆祝圣诞节；基督教的另一大分支——东正教的圣诞节庆则在每年的1月7日。
</p>
<p>圣诞节也是西方世界以及其他很多地区的公共假日，例如：在亚洲的中国香港和澳门地区、马来西亚、新加坡。
</p>

<img alt="圣诞节" src="https://dss2.baidu.com/6ONYsjip0QIZ8tyhnq/it/u=137662163,2033337145&fm=58">
<a href="#history">节日历史</a>
<a href="#customCelebration">习俗庆祝</a>
<a href="#socialInfluence">社会影响</a>

<hr/>
<div id="history">
    <h2>节日历史</h2>
    <p>
        据说耶稣是因着圣灵成孕，由圣母玛利亚所生的。神便派遣使者加伯列在梦中晓谕约瑟，叫他不要因为玛利亚未婚怀孕而不要她，反而要与她成亲，把那孩子起名为“耶稣”，意思是要他把百姓从罪恶中救出来。
        当玛利亚快要临盆的时候，罗马政府下了命令，全部人民到伯利恒务必申报户籍。约瑟和玛利亚只好遵命。他们到达伯利恒时，天色已昏，无奈两人未能找到旅馆渡宿，只有一个马棚可以暂住。就在这时，耶稣要出生了。于是玛利亚唯有在马槽上，生下耶稣。后人为纪念耶稣的诞生，便定十二月二十五为圣诞节，年年望弥撒，纪念耶稣的出世。
    </p>
    <p>
        4世纪初，1月6日是罗马帝国东部各教会纪念耶稣降生和受洗的双重节日、称为“主显节”（Epiphany），亦称“显现节”，即上帝通过耶稣向世人显示自己。当时只有那路拉冷的教会例外，那里只纪念耶稣的诞生而不纪念耶稣的受洗。后历史学家在罗马基督徒习用的日历中发现公元354年12月25日页内记录着：“基督降生在犹大的伯利恒。”经研究，一般认为12月25日伴为圣诞节可能开始于公元336年的罗马教会，约在公元375年传到小亚细亚的安提阿，公元430年传到埃及的亚历山大里亚，那路撒冷的教会接受得最晚，而亚美尼亚的教会则仍然坚持1月6日主显节是耶稣的诞辰。
        12月25日本是波斯太阳神（即光明之神）密特拉（Mithra）的诞辰，是一个异教徒节日，同时太阳神也是罗马国教众神之一。这一天又是罗马历书的冬至节，崇拜太阳神的异教徒把这一天当作春天的希望，万物复苏的开始。基于此原因，罗马教会选择这一天作为圣诞节。这是教会初期力图把异教徒的风俗习惯基督教化的措施之一。后来，虽然大多数教会都接受12月25日为圣诞节，但又固各地教会使用的历书不同，具体日期不能统一，于是就把12月24日到第二年的1月6日定为圣诞节节期（Christmas
        Tide），各地教会可以根据当地具体情况在这段节期之内庆祝圣诞节。自从12月25日被大多数教会公认为圣诞节后，原来1月6日的主显节就只纪念耶稣受洗了，但天主教会又把1月6日定为“三王来朝节”，以纪念耶稣生时东方三王（即三位博士）来朝拜的故事。随着基督教的广泛传播，圣诞节已成为各教派基督徒，甚至广大非基督徒群众的一个重要节日。
    </p>

    <p>
        但《圣经》中却从未提及耶稣出生在这一天，甚至很多历史学家认为耶稣是出生在春天。直到3世纪，12月25日才被官方定为圣诞节。尽管如此，还是有一些东正教把1月6日、7日定为圣诞节。 [3]
        一千三百多年前的腊月，唐代宗于大明宫为景教徒庆贺耶稣的降诞之日，他向教徒们分发香饼，大开筵席以飨僧众。这是史料中仅有的一句关于唐代的圣诞节的记载。这一瞬间被永远铭刻于公元781年，德宗敕建的“大秦景教流行中国碑”上 [4]
        。根据《序听迷诗所经》，当时的耶稣翻译为“移鼠”，“末艳”即圣母玛利亚，而“凉风”即是圣灵 [4] 。
        圣诞节本是宗教节日。十九世纪，圣诞卡的流行、圣诞老人的出现，使圣诞节开始渐渐流行起来。圣诞庆祝习俗在北欧流行后，结合着北半球冬季的圣诞装饰也出现了。 [5]
        十九世纪初发展至中叶，整个欧洲、美洲开始过起了圣诞节。并衍生出了相应的圣诞文化。
        圣诞节传播到亚洲是在十九世纪中叶，日本、韩国、中国等都受到了圣诞文化的影响。
        改革开放后，圣诞节在中国传播地尤为突出，至二十一世纪初，圣诞节有机地结合了中国当地习俗，发展日趋成熟。吃苹果、带圣诞帽、寄送圣诞贺卡，参加圣诞派对，圣诞购物等成了中国人生活的一部分。
    </p>
</div>
<div id="customCelebration">

    <h2>习俗庆祝</h2>

    <p>
        <strong>圣诞卡</strong>
        圣诞贺卡作为圣诞节礼物在美国和欧洲很流行，许多家庭随贺卡带上年度家庭合照或家庭新闻，新闻一般包括家庭成员在过去一年的优点特长等内容。圣诞节这天寄赠圣诞贺卡，除表示庆贺圣诞的喜乐外，就是向亲友祝福，以表思念之情。尤其对在孤寂中的亲友，更是亲切的关怀和安慰。
        装饰
    </p>
    <p>
        <strong>圣诞袜</strong>
        最早以前是一对红色的大袜子，大小不拘。因为圣诞袜是要用来装礼物的，所以是小朋友最喜欢的东西，晚上他们会将自己的袜子挂在床边，等待第二天早上收礼。 [5]
    </p>
    <p>
        <strong>圣诞帽</strong>
        是一顶红色帽子，据说晚上戴上睡觉除了睡得安稳和有点暖外，第二天你还会发现在帽子里多了点心爱的人送的礼物。
    </p>

    <p>
        <strong>圣诞树</strong>
        圣诞树（Christmas tree）是圣诞节庆祝中最有名的传统之一。通常人们在圣诞前后把一棵常绿植物如松树弄进屋里或者在户外，并用圣诞灯和彩色的装饰物装饰。并把一个天使或星星放在树的顶上。
        用灯烛和装饰品把枞树或洋松装点起来的常青树，作为圣诞节庆祝活动的一部分。圣诞树起源于德国。很久以前，罗马异教徒就用常青树的树枝装饰房子，寓意度过寒冷冬季之后的生命轮回。到了16世纪，德国人开始把常青树放到家中进行装饰。到了19世纪末，欧洲移民把圣诞树带入了美国殖民地并逐渐流传于世界各地。

        德国人于每年12月24日，即亚当和夏娃节，在家里布置一株枞树（伊甸园之树），将薄饼干挂在上面，象征圣饼（基督徒赎罪的标记）。近代改用各式小甜饼代替圣饼，还常加上象征基督的蜡烛。此外，室内还设有圣诞塔，是一木质的三角形结构，上有许多小架格放置基督雕像，塔身饰以常青树枝叶、蜡烛和一颗星。到16世纪，圣诞塔和伊甸园树合并为圣诞树。
        圣诞树到底是什么树呢？其实，只要是松柏类、常绿、树形呈三角形的树都可作为圣诞树。

    </p>
    <p>
        <strong>圣诞节橱窗</strong>
        圣诞橱窗也是墨尔本一道靓丽的风景线，每年的圣诞节来临前商店的橱窗设计人员就会动足脑筋，将这个圣诞节的主题发挥得淋漓尽致，而且绝不会和往年的风格重合，这里也是妈妈最愿意带孩子们来的地方。圣诞爷爷醇厚的嗓音讲述着惊心动魄的经历，故事还是那个故事，但声、光、电的组合更生动有趣。排队入场是玛雅橱窗参观中不成文的规定，栏杆外是急匆匆路过的人流，栏杆内有序参观，每个橱窗有数分钟的演绎。每个橱窗左下角是滚动的屏幕，立体声喇叭中讲述的故事，都能在这里显示，扫描一下二维码还能下载。


    </p>
    <p>
        <strong>圣诞节环</strong>
        西方国家圣诞节其间挂在家门口用的装饰品，通常用绿色的枝叶或藤条（松毛、松针等）和银色的金属及金色的铃铛配以红色的缎带组成主色调绿、白、黄、红代表欢乐喜庆上面写着MERRY CHRISTMAS或者简写为X'mas
        圣诞节环最早出现在芬兰。
    </p>


</div>

<div id="socialInfluence">
    <h2>社会影响</h2>
    <h4>经济</h4>
    <p>
        全球
        2012年，在全球经济不景气的情况下，全球的圣诞经济并不乐观。虽然较平常确有不小幅度的升温，但远远低于历史水平。尤其是类似希腊这样陷入债务危机的国家，经济本身并没有复苏，购物的人们只能转转无奈离去。英国、加拿大、新加坡、美国等国由于经济好转，在商家的大力促销下圣诞经济快速回升。
        [20]
        中国
        圣诞节对于没有基督文化背景的中国人来说，只是提供了购物或是又一个出国游玩的时间点罢了。中国国内众多城市都有了圣诞狂欢，商场、超市等在圣诞前后都有大型促销活动。也催生出了一个现象：“浙江义乌，号称世界圣诞饰品之都。”全球70%的圣诞饰品都来自这里。
        [21]
        2011年圣诞前后，众多中国人纷涌至英国各大城市购物，英国国内所售奢侈品的近三分之一都被中国人买走。在这种令人乍舌的购买力引导之下，不少国家在圣诞节专门推出针对中国人的有消费优惠的旅游计划。而英国伦敦更是有不少商家在圣诞节前后，专门雇佣会说普通话的店员，帮助中国顾客选购商品。2010年，中国内地游客在英国消费总量超过10亿英镑，英国本国居民的奢侈品消费需求则不足中国游客的一半。
        [21]

    </p>
    <h4>文化</h4>
    <p>宗教→全球性
        从最初的宗教节日，发展成为一个具有全球性的节日。圣诞节宗教涵义逐渐与世界各地文化传统糅合。有些是在宗教文化基础上演化，成为更加丰富多彩的圣诞节宗教文化。有些则逐渐世俗化、商业化，甚至政治化。
        以圣诞树而言，在希腊传统中是没有圣诞树的，但这并不代表圣诞节不能有或者不须有圣诞树。美国有摆放圣诞树的传统。西方国家的许多孩子从小就被告知，圣诞老人是从烟囱进入屋里，然后悄悄把礼物放在好孩子床头的袜子里。孩子们一旦功课成绩下降，就往往会被家长或者老师训诫可能得不到圣诞老人的礼物。美国纽约上州一名老师上月底在课堂上告诉学生“世上并没有圣诞老人”，还补充说圣诞树下的礼物是他们的父母放在那里的，就因引发家长争议而被迫道歉。

        单一→多元化
        圣诞节宗教神秘感的逐渐淡化，固然与科学发展有关，也与商品经济有关。市场经济下可以用各种赢利的形式包装圣诞节，商家使出各式各样的促销手段吸引消费者购买商品，圣诞节在使人们获得更多节日消费的理由的同时，也增添更多节日闲聊的谈资——消费文化。
        圣诞节文化的多元取向，使世界更精彩。
    </p>

</div>
</body>
</html>

```



#### 5.4.0 表格标签

> 表格主要用于显示/展示数据,因为它可以让数据显示的非常的规整,可读性非常好,特别是后台展示数据的时候,能够熟练运用表格就显得尤为重要.一个清爽简约的表格可以使繁杂的数据表现的很有条理性.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>表格标签</title>
</head>
<body>
<!-- table标签声明一个表格-->
<table>
    <!-- tr代表一行,td代表一列-->
    <tr>
        <td>id</td>
        <td>name</td>
        <td>age</td>
    </tr>
    <tr>
        <td>1</td>
        <td>张三</td>
        <td>12</td>
    </tr>
    <tr>
        <td>2</td>
        <td>李四</td>
        <td>15</td>
    </tr>
</table>
<table>
    <tr>
        <!-- th表示表头单元格标签,table head的缩写,在th中的文本会居中加粗显示-->
        <th>id</th>
        <th>name</th>
        <th>age</th>
    </tr>
    <tr>
        <td>1</td>
        <td>张三</td>
        <td>12</td>
    </tr>
    <tr>
        <td>2</td>
        <td>李四</td>
        <td>15</td>
    </tr>
</table>
</body>
</html>

```



#### 5.4.1 表格案例

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>表格案例</title>
</head>
<body>
<table border="8">
    <tr>
        <th>排名</th>
        <th>关键词</th>
        <th>今日搜索</th>
        <th>最近七日</th>
        <th>链接</th>
    </tr>
    <tr>
        <td>1</td>
        <td>鬼吹灯</td>
        <td>345</td>
        <td>123</td>
        <td>
            <a href="#">贴吧</a>
            <a href="#">百科</a>
        </td>
    </tr>
    <tr>
        <td>2</td>
        <td>盗墓笔记</td>
        <td>345</td>
        <td>123</td>
        <td>
            <a href="#">贴吧</a>
            <a href="#">百科</a>
        </td>
    </tr>

</table>


</body>
</html>
```



#### 5.4.2 表格结构标签

> 适用场景:因为表格可能非常长,为了更好地表达表格的语义,可以将表格分为表格头部和表格主题两大部分.
>
> 在表格标签中,分别用`<thead>`表示表格的头部区域,`<tbody>`表示表格的主题区域,以更好的分清表格结构

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>表格结构标签</title>
</head>
<body>
<table border="8">
    <thead>
        <tr>
            <th>排名</th>
            <th>关键词</th>
            <th>今日搜索</th>
            <th>最近七日</th>
            <th>链接</th>
        </tr>
    </thead>

    <tbody>
        <tr>
            <td>1</td>
            <td>鬼吹灯</td>
            <td>345</td>
            <td>123</td>
            <td>
                <a href="#">贴吧</a>
                <a href="#">百科</a>
            </td>
        </tr>
        <tr>
            <td>2</td>
            <td>盗墓笔记</td>
            <td>345</td>
            <td>123</td>
            <td>
                <a href="#">贴吧</a>
                <a href="#">百科</a>
            </td>
        </tr>
    </tbody>

</table>


</body>
</html>

```



![image-20201214211246501](https://raw.githubusercontent.com/zhangyutongdeyonghuming/web-design-learned/main/resources/image-20201214211246501.png).



#### 5.4.3 合并单元格

> 特殊情况下,可以把多个单元格合并为一个单元格.

![image-20201214211453389](https://raw.githubusercontent.com/zhangyutongdeyonghuming/web-design-learned/main/resources/image-20201214211453389.png).



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>表格合并单元格</title>
</head>
<body>
<table align="center" border="8">
    <thead>
        <tr>
            <td style="width:90px;" colspan="5">个人简历</td>
        </tr>
    </thead>

    <tbody>
        <tr>
            <td style="width:90px;">姓名</td>
            <td style="width:90px;"></td>
            <td style="width:90px;">性别</td>
            <td style="width:90px;"></td>
            <td style="width:90px;" rowspan="4">照片</td>
        </tr>
        <tr>
            <td style="width:90px;">婚姻状况</td>
            <td style="width:90px;"></td>
            <td style="width:90px;">出生年月</td>
            <td style="width:90px;"></td>
        </tr>
        <tr>
            <td style="width:90px;">民族</td>
            <td style="width:90px;"></td>
            <td style="width:90px;">政治面貌</td>
            <td style="width:90px;"></td>
        </tr>
        <tr>
            <td style="width:90px;">身高</td>
            <td style="width:90px;"></td>
            <td style="width:90px;">学历</td>
            <td style="width:90px;"></td>
        </tr>
    </tbody>
</table>


</body>
</html>
```



#### 5.4.4 列表标签

> 表格是用来显示数据的,列表标签是用来布局的.
>
> 列表的最大特点就是整齐/整洁/有序,它作为布局会更加的自由和方便.

##### 5.4.4.1 无序列表

> `<ul><li></li></ul>`,无序列表没有顺序,`<ul>`标签中只能嵌套`<li>`标签

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>无序列表标签</title>
</head>
<body>
    <p3>喜欢的食物</p3>
    <ul>
        <li>榴莲</li>
        <li>臭豆腐</li>
        <li>鲱鱼罐头</li>
        <li>臭鳜鱼</li>
    </ul>
</body>
</html>

```



##### 5.4.4.2 有序列表

> 有序列表使用在有排列顺序的列表,语法为`<ol><li></li></ol>`,`<ol>`标签中只能嵌套`<li>`标签

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>列表标签</title>
</head>
<body>
    <h2>喜欢的明星</h2>
    <ol>
        <li>刘德华</li>
        <li>黎明</li>
        <li>张学友</li>
        <li>郭富城</li>
    </ol>
</body>
</html>

```



##### 5.4.4.3 自定义列表

> 自定义列表常用语对术语/名字进行解释或描述,自定义列表的列表项前没有项目符号.
>
> `<dl>`
>
> ​	`<dt>标题</dt>`
>
> ​	`<dd>内容</dd>`
>
> `</dl>`
>
> dl里只能写dt/dd

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>列表标签</title>
</head>
<body>
<!--自定义列表-->
    <dl>
        <dt>关注我们</dt>
        <dd>官方微博</dd>
        <dd>官方微信</dd>
        <dd>联系我们</dd>
        <dt>关注我们</dt>
        <dd>官方微博</dd>
        <dd>官方微信</dd>
        <dd>联系我们</dd>
    </dl>
</body>
</html>

```



##### 5.4.4.5 列表总结

| 标签        | 定义       |
| ----------- | ---------- |
| `<ul></ul>` | 无序标签   |
| `<ol></ol>` | 有序标签   |
| `<dl></dl>` | 自定义标签 |



#### 5.4.5 表单标签

> 使用表单是为了方便**收集用户信息**.
>
> 在网页中需要与用户进行交互,收集用户资料,此时就需要表单.
>
> 表单由表单域/表单控件(表单元素)和提示信息构成

![image-20201215203433022](https://raw.githubusercontent.com/zhangyutongdeyonghuming/web-design-learned/main/resources/image-20201215203433022.png).

> 表单域是一个包含表单元素的区域,以`<form>`标签包含起来,提交时会将范围内的表单元素信息提交给服务器.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>表单域</title>
</head>
<body>
    <form action="/action" method="get" name="name">

    </form>
</body>
</html>
```



> 表单元素(表单控件)
>
> 在表单域中可以定义各种表单元素,这些元素就是允许用户在表单中输入或者选择的内容控件.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>表单元素</title>
</head>
<body>

<form action="/req" method="get">
    <!--    text 文本框 使用placeholder可以显示信息,maxlength指定值最大长度-->
    用户名:<input type="text" placeholder="请输入用户名" maxlength="10"/> <br>
    <!--    password 密码-->
    密码:<input type="password"/> <br>
    <!--    radio 单选按钮,单选按钮互斥只需指定同一个name属性即可,value只可以分男女-->
    性别: 男<input type="radio" checked name="sex" value="男"/> 女<input type="radio" name="sex" value="女"/> <br>
    <!--    checkbox 复选框-->
    爱好: 
    篮球 <input type="checkbox" checked name="hobby"/>
    足球 <input type="checkbox" name="hobby"/>
    长歌 <input type="checkbox" name="hobby"/>

</form>
</body>
</html>

```

> `<input>`属性



| 属性      | 属性值  | 描述                                                 |
| --------- | ------- | ---------------------------------------------------- |
| name      | 自定义  | 定义input元素的名称,后台可以拿到的key-value其中的key |
| value     | 自定义  | 定义元素的值                                         |
| checked   | checked | 定义加载时是否被选中                                 |
| maxlength | 正整数  | 定义字段值最大长度                                   |



> label标签为input元素定义标注
>
> 用于绑定一个表单元素,当点击label标签内的文本时,浏览器会自动将焦点转到或者选择对应的表单元素上,用来增加用户体验.



```hrml
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>label</title>
</head>
<body>
<form action="">
	<!-- 点击用户名即可输入-->
    <label for="username">用户名:</label>
    <input id="username" type="text"/>
    <br>
    性别:
    <!-- 点击汉字即可选择男/女-->
    <input id="boy" type="radio" name="sex"><label for="boy">男</label>
    <input id="girl" type="radio" name="sex"><label for="girl">女</label>
</form>
</body>
</html>
```



> 下拉标签
>
> 适用场景:在页面中如果有多个选项让用户选择,并且想要节约页面空间时,我们可以使用`<select>`标签定义下拉列表



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>select</title>
</head>
<body>
    <form>
        籍贯:
        <select name="address" id="address">
            <!-- selected默认选中-->
            <option value="" selected>北京</option>
            <option value="">河南</option>
            <option value="">河北</option>
            <option value="">南京</option>
        </select>
    </form>
</body>
</html>

```



> textarea标签
>
> 适用场景:个人简介/留言等大量文字场景

```html
<html>
<head>
    <meta charset="UTF-8">
    <title>textarea</title>
</head>
<body>

<form action="">
    <textarea name="" id="" cols="30" rows="10">留言板...
    </textarea>
</form>

</body>
</html>
```



> 综合案例

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>综合案例:注册页面</title>
</head>
<body>
<table>
    <form action="">
        <tr>
            <td colspan="2">青春不常在,赶紧谈恋爱</td>
        </tr>

        <tr>
            <td>性别</td>
            <td>
                <input type="radio" name="sex" id="boy"/> <label for="boy">男</label>
                <input type="radio" name="sex" id="girl"/> <label for="girl">女</label>
            </td>
        </tr>

        <tr>
            <td>生日</td>
            <td>
                <select name="">
                    <option value="" selected>请选择年</option>
                </select>

                <select name="">
                    <option value="" selected>请选择月</option>
                </select>

                <select name="">
                    <option value="" selected>请选择日</option>
                </select>
            </td>
        </tr>

        <tr>
            <td>所在地区</td>
            <td>
                <input type="text"/>
            </td>
        </tr>

        <tr>
            <td>喜欢类型</td>
            <td>
                <input id="charming" type="checkbox"/> <label for="charming">妩媚的</label>
                <input id="pure" type="checkbox"/> <label for="pure">清纯的</label>
                <input id="lovely" type="checkbox"/> <label for="lovely">可爱的</label>
            </td>

        </tr>

        <tr>
            <td>自我介绍</td>
            <td>
                <textarea name="" id="" cols="30" rows="10">

                </textarea>
            </td>
        </tr>

        <tr>
            <td colspan="2">
                <input type="submit"/>
            </td>
        </tr>
    </form>
</table>
</body>
</html>

```



### 6. CSS层叠样式表

>**HTML的局限性**:HTML只关注内容的语义,并不关注内容的样式,虽然可以用做简单的样式,但是带来的是无尽的繁琐及臃肿
>
>**CSS**:是层叠样式表(Cascading Style Sheets)的简称,也是一种标记语言,主要用于设置HTML页面中的文本内容(字体/大小/对齐方式等)/图片的外形(宽高/边框/边距)及版面的布局和外观显示样式.CSS可以美化HTML,使页面更漂亮.
>
>**CSS语法规范**:CSS选择器 { 属性: 值;},如h1{color:red;}



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>css初体验</title>
    <style>
        /* css都写在style标签里 */
        /* 给谁该样式{样式:样式值} */
        p {
            /* 修改字体颜色 */
            color: red;
            /* 修改字体大小 */
            font-size: 50px;
        }
    </style>
</head>
<body>
    <p>
        有点儿意思
    </p>
</body>
</html>
```



#### 6.1 CSS基础选择器

> 选择器的作用:用于选择标签.



##### 6.1.1 标签选择器:

> 标签名 { 属性: 属性值;}

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>标签选择器</title>
    <style>
        /* 选中页面里所有div */
        div {
            color: red;
            font-size: 25px;
        }
        /* 选中页面里所有的p标签 */
        p {
            color: pink;
            font-size: 50px;
        }
    </style>
</head>
<body>
    
    <p>爱是一道光</p>
    <div>绿到你发慌</div>
    <div>来顶帽子吧</div>
    <p>给你一顶帽子</p>
</body>
</html>
```



##### 6.1.2 类选择器

> 选中所有class属性相同的标签, .class { 属性: 属性值;}

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>类选择器</title>
    <style>
        /* 选择所有class等于red的元素 */
        .red {
            color: red;
            font-size: 23px;
        }
    </style>
</head>
<body>
    <ol>
        <li class="red">red</li>
        <li class="red">red</li>
        <li class="red">red</li>
        <li class="black">black</li>
        <li class="black">black</li>
    </ol>
    <div class="red">我也是红色</div>
</body>
</html>
```



> 多类名
>
> 一个标签可以使用多个类名

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>案例</title>
    <style>
        /* 可以使用这个来给3个都设置属性 */
        .box {
            width: 200px;
            height: 200px;
        }
        .red {
            background-color: red;
        }
        .green {
            background-color: green;
        }
    </style>
</head>
<body>
    <div class="red box"></div>
    <div class="green box"></div>
    <div class="red box"></div>
</body>
</html>
```



##### 6.1.3 id选择器

> id全页面唯一
>
> #id { 属性: 属性值;}

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>案例</title>
    <style>
        #green {
            font-size: 50px;
            color: green;
        }
        #red {
            font-size: 12px;
            color: red;
        }

        
    </style>
</head>
<body>
    <ol>
        <li id="green">张三</li>
        <li id="red">李四</li>
    </ol>
</body>
</html>
```



6.1.4 通配符选择器

> 在CSS中,通配符使用*****号定义.
>
> *{ 属性: 属性值;}

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>*</title>
    <style>
        /* 选择所有标签 */
        * {
            margin: 0;
            padding: 0;
            color: brown;
        }
    </style>
</head>
<body>
    <div>测试文本</div>
</body>
</html>
```



#### 6.2 CSS字体属性

> CSS Fonts属性用于定义字体系列,大小,粗细和文本样式

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>字体属性系列</title>
    <style>
        h3 {
            /* font-family可以设置字体. */
            font-family: '微软雅黑';
            /* font-size可以设置字体大小 */
            font-size: 30px;
        }

        p {
            /* 可以设置多个字体 */
            font-family: Arial,'Microsoft YaHei';
        }
        .bold {
            /* font-weight默认是normal,
            bold 同strong标签 
            开发者常用数字表示粗细,没有单位.
            */
            font-weight: bold;
            /* 等价font-weight: 700; */
        }
        .normal {
            font-weight: normal;
            /* 等价font-weight: 400; */
        }
        .italic {
            /* 斜体 */
            font-style: italic;
        }
        em {
            /* 斜体变正常 */
            font-style: normal;
        }
        #allStyle {
            /*  
                font-style: italic;
                font-weight: 700;
                font-size: 16px;
                font-family: 'Microsoft YaHei'; 
            */
            /* 字体复合属性,将上述几行合为一行,顺序不能更改 */
            /* font: font-style font-weight font-size font-family */
            /* font: italic 700 16px 'Microsoft YaHei' */
            /* font-style/font-weight可以缺省 */
            font: 22px 'Microsoft YaHei'
        }
    </style>
</head>
<body>
    <!-- 浪漫的李白.-->
    <h3 class="normal">清平乐·画堂晨起</h3>
    <em>李白</em>
    <p id="allStyle">画堂晨起，来报雪花坠。</p>
    <p>高卷帘栊看佳瑞，皓色远迷庭砌。</p>
    <p class="italic">盛气光引炉烟，素草寒生玉佩。</p>
    <p class="bold">应是天仙狂醉，乱把白云揉碎。</p>
    
</body>
</html>
```



> 字体属性总结

| 属性        | 表示         | 注意点                                                       |
| ----------- | ------------ | ------------------------------------------------------------ |
| font-style  | 字体样式     | 斜体是italic,不倾斜默认是normal                              |
| font-weight | 字体粗细     | bold是700,不加粗是normal/400,一般用数字                      |
| font-size   | 字体大小     | 通常以px为单位                                               |
| font-family | 字体         | 默认以浏览器字体,使用时需注意带空格的加引号如'Microsoft YaHei' |
| font        | 字体集合属性 | 格式: font: font-style font-weight font-size font-family ,前两个属性可以缺省,但顺序不可变 |



#### 6.3 CSS文本属性

> CSS Text属性可以定义文本的外观,比如文本颜色,对齐,装饰文本,缩进,行间距.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>文本属性</title>
    <style>
        div {
            /* color 设置文本颜色 */
            /* color: red; */
            /* color: rgb(200,0,0); */

            /* 十六进制最常用,因为需要ps吸取颜色. */
            color: #ff0000;

            /* left左对齐(default);right右对齐;center居中对齐 */
            text-align: right;
        }

        a {
            /* 可以取消a标签的下划线,最常用 */
            text-decoration: none;
        }

        #line {
            /* 下划线 */
            /* text-decoration: underline; */

            /* 上划线 */
            /* text-decoration: overline; */

            /* 删除线 */
            text-decoration: line-through;
        }

        p {
            /* 首行缩进,可以使用px/em,em指代当前元素一个文字大小 */
            /* text-indent: 24px; */
            text-indent: 2em;
            /* 设置行高 */
            line-height: 36px;
        }
    </style>
</head>

<body>
    <div>听说下雨天和巧克力更配哦</div>
    <a href="http://baidu.com" target="_black">百度</a>
    <div id="line">测试上下滑线</div>

    <p>央视网消息（新闻联播）：国务院新闻办今天（12月17日）举行发布会，自然资源部、国家发展改革委等部门相关负责人在会上表示，“十三五”期间，我国生态保护修复工作成绩显著。生态保护修复法律制度加快完善，自然保护地体系建设稳步推进。截至目前，建立各类自然保护地1.18万个，约占我国陆域国土面积的18%。在12省份开展了国家公园试点，总面积超过22万平方公里。</p>
    <p>国家还在重点生态功能区实施了25个山水林田湖草生态保护修复试点工程，有效解决了生态退化问题。此外，全国国土绿化“十三五”规划主要任务全面完成，森林覆盖率达到23.04%。</p>
</body>

</html>
```



| 属性            | 表示     | 注意点                                                       |
| --------------- | -------- | ------------------------------------------------------------ |
| color           | 文本颜色 | 通常用#十六进制表示                                          |
| text-align      | 文本对齐 | 设定文字对齐方式                                             |
| text-indent     | 文本缩进 | 通常缩进两个字为:text-indent: 2em;                           |
| text-decoration | 文本修饰 | a标签可以使用text-decoration: none;来取消下划线;none 默认,没有装饰线;underline 下划线;overline 上划线;line-through 删除线. |
| line-height     | 行高     | 控制行之间的距离,行高计算: 上间距 + 下间距 + 文字大小.       |



#### 6.4 样式表引入方式

| 样式表     | 使用情况                                         | 控制范围     |
| ---------- | ------------------------------------------------ | ------------ |
| 行内样式表 | 书写方便,但结构样式混乱,使用较少                 | 控制一个标签 |
| 内部样式表 | 部分结构和样式相分离,但没有彻底分离,使用较多     | 控制一个页面 |
| 外部样式表 | 完全实现结构与样式分离,是封装组件的基础,使用最多 | 控制多个页面 |



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>css引入方式</title>

    <!-- 外联样式表 -->
    <link rel="stylesheet" href="02-css引入方式.css">

    <!-- 内部样式表 -->
    <style>
        div {
            color: red;
        }
    </style>
</head>
<body>

    <div>所谓新闻</div>
    

    <!-- 行内样式/内联样式 -->
    <p style="line-height: 36px;text-indent: 2em">
        中新社巴黎12月17日电 (记者 李洋)法国总统马克龙当地时间17日晚在确诊感染新冠病毒后首次露面。法国官方当晚披露了马克龙感染病毒的具体症状，引发外界高度关注。
    </p>

    <p id="pink">粉红的回忆</p>
</body>
</html>
```



#### 6.5 综合案例

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>中国新闻网</title>
    <!-- 引入外部样式表 -->
    <link rel="stylesheet" href="./03-css综合案例.css">
</head>

<body>
    <h1>马克龙确诊感染后首次露面 法国官方披露具体症状
    </h1>

    <div class="author">
        2020年12月18日 06:00　来源：<a target="_black" href="http://www.chinanews.com/">中国新闻网</a>
    </div>

    <p>
        中新社巴黎12月17日电 (记者 李洋)法国总统马克龙当地时间17日晚在确诊感染新冠病毒后首次露面。法国官方当晚披露了马克龙感染病毒的具体症状，引发外界高度关注。
    </p>
    <div class="images">
        <img alt="马克龙" src="http://i2.chinanews.com/simg/cmshd/2020/12/18/a52b9560ee07439598b304936f5a6329.jpg">
    </div>

    <p>
        马克龙当晚通过视频连线的方式出席人道主义援助政策会议并发表十多分钟的讲话。法国外长勒德里昂等与会者在法国外交部的会议主会场聆听马克龙的视频讲话。
    </p>

    <p>马克龙在讲话期间偶尔查看讲话文稿，思路仍然清晰，吐字清楚。他讲话全程都戴着防护口罩，也没有戴领带。他在讲话中没有具体谈及个人情况。法国多家电视台对马克龙的讲话进行了直播。</p>
    <div class="images">
        <img src="http://i2.chinanews.com/simg/cmshd/2020/12/18/b98dc14042954fc5bbc131cb1c6af4fc.jpg" alt="">
    </div>
    <p>
       法国政府发言人阿塔尔当晚代表官方对外披露马克龙感染病毒的具体症状。他说，马克龙具有这种疾病的“真实症状”，即“咳嗽和严重疲劳”。阿塔尔表示，马克龙目前仍然可以通过视频会议的方式继续参加很多活动。
    </p>  

    <p>
       马克龙当天通过新冠病毒检测确诊感染。阿塔尔稍早前透露，他16日深夜感到有症状，立即进行自我隔离。他随后接受病毒检测，结果为阳性。阿塔尔确认马克龙遵守社交距离的相关规定，并表示他将远程办公。
    </p>

    <p>
        法国总理卡斯泰、国民议会议长费朗等法国政要因16日曾与马克龙会面并共进晚餐而接受隔离。卡斯泰已取消了17日的公开行程，也改为远程办公。
    </p>
    
    <p>
        记者当天前往法国总统府爱丽舍宫和总理府马提尼翁宫查看情况。两处地点从外部看都运转如常。爱丽舍宫外的警力略有增加。在爱丽舍宫外聚集了大批媒体记者，多名电视主持人在做现场连线；马提尼翁宫只有两名记者在蹲守。
    </p>

    <p>
        马克龙最近两周行程安排紧凑，过去三天中每天都有多场活动。最近曾与马克龙在相关场合会面的西班牙首相桑切斯、葡萄牙总理科斯塔、比利时首相德克罗、欧洲理事会主席米歇尔等政要17日均接受隔离。(完)
    </p>

<div class="author editor">【编辑:田博川】</div>
</body>

</html>
```

```css

h1 {
    font-weight: 500;
}

p {
    line-height: 40px;
    text-indent: 2em;
    font-size: 20px;
}

a {
    text-decoration: none;
    color: #a3a3a3;
}

.author {
    color: #666666;
    font-size: 14px;
}

.editor {
    text-align: right;
}

.images {
    text-align: center;
}
```



#### 6.6 CSS复合选择器

>在CSS中可以根据选择器类型分为基础选择器和复合选择器,复合选择器是建立在基础选择器之上,对基本选择器进行组合形成的
>
>- 复合选择器可以更准确的/更高效的选择目标元素;
>- 复合选择器是由两个或多个基础选择器,通过不同的方式组合而成的;
>- 常用的复合选择器包括: 后代选择器/子选择器/并集选择器/伪类选择器等



##### 6.6.1 后代选择器

> 后代选择器又称包含选择器, 可以选择父元素里面的子元素 .其写法就是把外层标签写在前面, 内层标签写在后面, 中间用空格分隔. 当标签发生嵌套时, 内层标签就成为外层标签的后代.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 后代选择器: 父标签 空格 子标签 {} */
        ol li {
            color: green;
        }

        ul li {
            /* 去除无序列表的圆圈 */
            list-style: none;
        }

        /* 可以用类/id选择器来选择,可以是任意基础选择器 */
        .blue li {
            color: blue;
        }
    </style>
</head>

<body>
    <ol>
        <li>我是ol的孩子</li>
        <li>我是ol的孩子</li>
        <li>我是ol的孩子</li>
    </ol>

    <ol class="blue">
        <li>我是ol的孩子</li>
        <li>我是ol的孩子</li>
        <li>我是ol的孩子</li>
    </ol>

    <ul>
        <li>我是ul的孩子</li>
        <li>我是ul的孩子</li>
        <li>我是ul的孩子</li>
    </ul>
</body>

</html>
```



##### 6.6.2 子选择器

> 子选择器只能选择作为某元素的最近一级子元素.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 子选择器,写法: 父>子 */
        div>a {
            color: brown;
            text-decoration: none;
        }

        .nav>a {
            color: bisque;
        }
    </style>
</head>

<body>
    <div>
        <a href="http://baidu.com">儿子</a>
    </div>

    <div>
        <p><a href="http://baidu.com">孙子</a></p>
    </div>

    <div class="nav">
        <a href="#">大肘子</a>
        <ul>
            <li><a href="#">baidu</a></li>
            <li><a href="#">baidu</a></li>
        </ul>
    </div>


</body>

</html>
```



##### 6.6.3 并集选择器

> 并集选择器可以选择多组标签, 同时为他们定义相同样式, 通常用于集体声明

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 使用逗号分隔多个选择,声明为并集选择器 */
        div,
        p,
        ul li {
            color: pink;
        }
    </style>
</head>

<body>
    <div>胸大</div>
    <p>熊二</p>
    <ul>
        <li>小猪佩奇</li>
        <li>猪八</li>
        <li>猪吗</li>
    </ul>
</body>

</html>
```



##### 6.6.4 伪类选择器

> 伪类选择器用于向某些选择器添加特殊的效果, 比如给链接添加特殊效果, 或选择第一个/第n个元素.
>
> 书写特点: 用冒号表示



###### 6.6.4.1 链接伪类选择器

>a:link 选择所有未被访问的链接;
>
>a:visited 选择所有已被访问的链接;
>
>a:hover 选择鼠标指针位于其上的链接;
>
>a:active 选择活动链接,鼠标按下未弹起
>
>注意事项:
>
>为了确保伪类选择器能够生效, 声明的顺序最好不要颠倒, 按照link-visited-hover-active的顺序来声明.
>
>因为a标签自带样式,所以在开发时需要给链接单独指定样式.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 为了确保伪类选择器能够生效, 声明的顺序最好不要颠倒, 按照link-visited-hover-active的顺序来声明.*/
        /* 选中没有访问过得a标签 */
        a:link {
            text-decoration: none;
            color: #333;
        }

        /* 已经访问过得链接 */
        a:visited {
            color: orange;
        }

        /* 鼠标滑过a标签 */
        a:hover {
            color: red;
        }

        /* 鼠标正在点击,没有松开时 */
        a:active {
            color: green;
        }
    </style>
</head>

<body>
    <a href="#" target="_black">百度</a>
</body>

</html>
```



###### 6.6.4.2 :focus伪类选择器

> 选择获得焦点的表单元素.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 选择获得焦点的表单元素 */
        input:focus {
            background-color: red;
        }
    </style>
</head>

<body>
    <input type="text" />
    <input type="text" />
    <input type="text" />
</body>

</html>
```



##### 6.6.5 复合选择器总结

| 选择器           | 作用                           | 用法                              |
| ---------------- | ------------------------------ | --------------------------------- |
| 后代选择器       | 选择后代元素                   | 使用空格隔开,如div a              |
| 子代选择器       | 选择最近一级元素               | 使用大于号隔开,如div>a            |
| 并集选择器       | 选择某些相同样式的元素集体声明 | 使用逗号隔开,如div,a              |
| 链接伪类选择器   | 选择不同状态的a标签链接        | a:link/a:visited/a:hover/a:active |
| :focus伪类选择器 | 选择获得焦点的表单元素         | input:focus                       |





#### 6.7 CSS的元素显示模式

> 网页标签繁多, 在不同的地方会用到不同类型的标签, 了解他们的特点可以更好的布局我们的网页.
>
> 元素显示模式就是元素以什么方式进行显示, 比如div 自己占一行, 比如一行可以放多个span
>
> HTML一般分为**块元素**和**行内元素**



##### 6.7.1 块级元素

> 常见块级元素有h1-h6/p/div/ul/ol/li等, 其中div是最典型的块级元素
>
> 块级元素的特点是:
>
> 1. 独占一行;
> 2. 高度/宽度/外边距/内边距可以控制;
> 3. 宽度默认是容器的100%;
> 4. 是一个容器及盒子, 里面可以放行内或块级元素
> 5. 文字类标签不能使用块级元素, 如p标签/h1-h6标签都是存放文字的, 里面不能放块级元素



```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>块级元素</title>
    <style>
        div {
            /* 不设置宽度 则默认使用父标签的宽度 */
            /* width: 200px; */
            height: 400px;
            background-color: aqua;
        }
    </style>
</head>

<body>
    <div>比较霸道,独占一行</div>
    瑟瑟发抖
    <!-- 这里会有问题 -->
    <p>
    <div>123</div>
    </p>
</body>

</html>
```





##### 6.7.2 行内元素

> 常见的行内元素有a/strong/b/em/i/del/s/ins/u/span等, 其中span是最典型的行内元素,有的地方也称其为内联元素.
>
> 特点:
>
> 1. 相邻行内元素在一行上, 一行可以显示多个;
> 2. 高/宽直接设置是无效的;
> 3. 默认宽度就是他本身内容的宽度;
> 4. 行内元素只能容纳文本或其他行内元素(a标签内不允许在套a标签, 但是a可以放块级元素)

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <span>老师好</span>
    <strong>好老师</strong>
</body>

</html>
```



##### 6.7.3 行内块元素

> 在行内元素中有几个特殊的标签----img/input/td, 他们同时具有块元素和行内元素的特点.
>
> 特点:
>
> 1. 和相邻行内元素在一行上,但是他们之间会有空白缝隙. 一行可以显示多个(行内元素特点);
> 2. 默认宽度就是本身内容的宽度(行内元素特点);
> 3. 高度, 行高, 外边距/内边距都可以控制(块级元素特点).

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        input {
            /* 可以设置高度/宽度 */
            width: 250px;
            height: 30px
        }
    </style>
</head>

<body>
    <!-- 一行可以显示多个,默认宽度为本身内容的宽度 -->
    <input type="text">
    <input type="text">
</body>

</html>
```



##### 6.7.4 元素显示模式总结



| 元素模式   | 元素排列               | 设置样式           | 默认宽度       | 包含                   |
| ---------- | ---------------------- | ------------------ | -------------- | ---------------------- |
| 块级元素   | 一行只能放一个块级元素 | 可以设置宽高       | 容器的100%     | 可以包含任何标签       |
| 行内元素   | 一行可以放多个行内元素 | 不可以直接设置宽高 | 本身内容的宽度 | 容纳文本或其他行内元素 |
| 行内块元素 | 一行放多个行内块元素   | 可以设置宽高       | 本身内容的宽度 |                        |



#### 6.8 CSS的元素显示模式转换

> 特殊情况下,我们需要元素模式的转换, 简单来说就是一个模式的元素需要另外一种模式的特性.
>
> 转为块元素: display: block; 
>
> 转为行内元素: display: inline;
>
> 转为行内块元素: display: inline-block;



```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        a {
            width: 150px;
            height: 50px;
            background-color: red;
            /* 把行内元素转为块元素 */
            display: block;
        }

        div {
            /* 行内元素 高/宽失效了 */
            width: 300px;
            height: 100px;
            background-color: pink;
            /* 把块级元素转换为行内元素 */
            display: inline;
        }

        span {
            width: 200px;
            height: 30px;
            background-color: blue;
            /* 把行内元素转为行内块 */
            display: inline-block;
        }
    </style>
</head>

<body>
    <a href="#">点击这里</a>

    <div>我是块级元素</div>
    <div>我是块级元素</div>

    <span>我是行内元素</span>
</body>

</html>
```



#### 6.9 元素模式案例

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>小米侧边栏丐版</title>
    <style>
        a {
            /* 转换为块级元素 */
            display: block;
            width: 234px;
            height: 54px;
            /* 取消下划线 */
            text-decoration: none;
            color: #fff;
            background-color: gray;
            /* 首行缩进2个字符 */
            text-indent: 2em;
            font-size: 14px;
            /* 由于css没提供垂直居中代码,所以使用小技巧实现 */
            line-height: 54px
        }

        /* 设置a标签滑过样式 */
        a:hover {
            background-color: orange;
        }
    </style>
</head>

<body>
    <a href="#">手机 电话卡</a>
    <a href="#">电视 盒子</a>
    <a href="#">笔记本 平板</a>
    <a href="#">出行 穿戴</a>
    <a href="#">智能路由器</a>
    <a href="#">健康 儿童</a>
    <a href="#">耳机 音响</a>
</body>

</html>
```



#### 6.10 CSS背景

##### 6.10.1 背景图片

> background-image  属性描述了元素的背景图像. 实际开发常见于logo或者是一些装饰性的小图片或者是超大的背景图片, 优点是非常便于控制位置. 精灵图也是一种运用场景.默认为none



```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        div {
            height: 300px;
            width: 300px;
            background-color: gray;
            /* 设置图片背景 , 默认none*/
            background-image: url(../resources/logo.png);
            /* 设置背景不平铺 */
            background-repeat: no-repeat;
            /* 设置方位,如果是名词则没有顺序 */
            background-position: center top;
        }
    </style>
</head>

<body>
    <div></div>
</body>

</html>
```



> 背景图片方位参数也可以是具体值

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        div {
            width: 430px;
            height: 161px;
            background-color: gray;
            background-repeat: no-repeat;
            background-image: url(../resources/logo.png);
            /* 可以指定固定的数值加单位来指定偏移量,顺序是先x轴后y轴,如果不指定第二个则默认垂直居中 */
            background-position: 50px;
        }
    </style>
</head>

<body>
    <div></div>
</body>

</html>
```



> 也可以进行混合使用

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body {
            background-image: url(../resources/725341110883827.jpg);
            /* 也可以使用混合单位,也是先x,后y */
            background-position: center 40px;
        }
    </style>
</head>

<body>
</body>

</html>
```



##### 6.10.2 背景图片固定

> background-attachment 属性设置背景图片是否固定或者随着页面的其余部分滚动, 可以做视差滚动的效果
>
> background-attachment: scroll | fixed

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body {
            background-image: url(../resources/725341110883827.jpg);
            background-position: center 40px;
            background-repeat: no-repeat;
            /* 固定背景图片, 不随下拉而滚动, 默认是scroll(滚动) */
            background-attachment: fixed;
        }

        p {
            color: #fff;
            font-size: 35px;
        }
    </style>
</head>

<body>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
    <p>提莫一米五</p>
</body>

</html>
```



##### 6.10.3 背景的复合写法

> 为了简化背景属性的代码, 我们可以简写在一个background中, background没有特定的书写顺序.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body {
            /* background-image: url(../resources/725341110883827.jpg); */
            /* background-position: center 40px; */
            /* background-repeat: no-repeat; */
            /* 固定背景图片, 不随下拉而滚动, 默认是scroll(滚动) */
            /* background-attachment: fixed; */

            /* 简化代码 */
            background: url(../resources/725341110883827.jpg) no-repeat fixed center 40px;
        }

        p {
            color: #fff;
            font-size: 35px;
        }
    </style>
</head>

<body>
</body>

</html>
```



##### 6.10.4 背景色半透明

> background: rgba(0,0,0,0.3) 可以设置背景色半透明, a是alpha透明度, 取值范围在0-1之间

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        div {
            height: 400px;
            width: 400px;
            background: rgba(0, 0, 0, 0.3);
        }
    </style>
</head>

<body>
    <div>123</div>
</body>

</html>
```



##### 6.10.4 背景总结

| 属性                  | 作用     | 值                                 |
| --------------------- | -------- | ---------------------------------- |
| background-color      | 背景颜色 | 预定义的颜色值/十六进制/RGB代码    |
| background-image      | 背景图片 | url(路径)                          |
| background-repeat     | 背景平铺 | repeat/no-repeat/repeat-x/repeat-y |
| background-position   | 背景位置 | length/position                    |
| background-attachment | 背景固定 | scroll(滚动)/fixed(固定)           |



#### 6.11 CSS三大特性

> CSS有三个非常重要的特性: 层叠性, 继承性, 优先级.



##### 6.11.1 层叠性

> 相同选择器给设置相同的样式, 此时一个样式就会覆盖另一个冲突的样式, 层叠性主要解决样式冲突的问题.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        div {
            color: aliceblue;
        }

        /* 就近原则, 最下边的覆盖上边的 */
        div {
            color: pink;
        }
    </style>
</head>

<body>
    <div>这是一个div</div>
</body>

</html>
```



##### 6.11.2 继承性

>CSS的继承: 子标签会继承父标签的某些样式, 如文本颜色和字号.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        div {
            color: blue;
            font-size: 20px;
        }
    </style>
</head>

<body>
    <div>我是div
        <!-- p继承了div的字号和颜色 -->
        <p>我是p</p>
    </div>
</body>

</html>
```



> 行高的继承

```html
body {
    /* 注意简写行高时必须指定font-family */
    font: 12px/1.5 Arial;
}
```

> - 行高可以跟单位也可以不跟单位;
> - 如果子元素没有行高, 则会默认继承父元素的行高;
> - 此时子元素的行高为: 当前子元素的**文字大小 * 父元素行高倍数**;
> - 这种写法的优点是子元素可以根据自己文字大小自动调整行高.





##### 6.11.3 优先级

> 当元素指定了多个选择器时,就会有优先级的产生.
>
> 选择器相同则执行层叠性;选择器不同则根据选择器权重执行.

| 选择器              | 选择器权重 |
| ------------------- | ---------- |
| 继承或者*           | 0,0,0,0    |
| 元素选择器          | 0,0,0,1    |
| 类选择器/伪类选择器 | 0,0,1,0    |
| ID选择器            | 0,1,0,0    |
| 行内样式: style=""  | 1,0,0,0    |
| !important          | 无穷大     |



```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body {
            /* 继承 */
            color: gray;
        }

        div {
            /* 元素选择器*/
            color: red;
        }

        .test {
            /* 类选择器 */
            color: pink;
        }

        #col {
            /* ID选择器 */
            color: orange;

        }

        div {
            /* !important 强制执行优先级无穷大.*/
            color: red !important;
        }
    </style>
</head>

<body>
    <div class="test" id="col" style="color:blue">你笑起来真好看</div>
</body>

</html>
```



> 优先级权重叠加: 如果使用复合选择器则会有权重叠加

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 使用复合选择器时权重叠加,比单标签选择权重高 */
        ul li {
            color: green;
        }

        li {
            color: blue;
        }
    </style>
</head>

<body>
    <ul>
        <li>大猪蹄子</li>
        <li>大鸡爪子</li>
    </ul>
</body>

</html>
```

























