---
layout: post
title: pinyin4j 声母与韵母的基础知识
date:  2020-1-9 10:09:32 +0800
categories: [Search]
tags: [nlp, index, math, pinyin, sh]
published: true
---

# 汉语拼音是拼写汉民族标准语的拼音方案。

汉语拼音是以北京语音系统作为语音标准的。

北京音也是中国地域最辽阔、人口最多的北方方言的典型代表。

解释汉语拼音用法和标准的《汉语拼音方案》是中国拼音文字方案的国家标准，也是联合国规定用来拼写中国人名地名和专用词语的国际标准。 

它是中华人民共和国法定的拼音方案，是世界文献工作中拼写有关中国的专用名词和词语的国际标准。

1958年2月11日，第一届全国人民代表大会第五次会议正式通过了《汉语拼音方案》，并批准公布推行。

《汉语拼音方案》是采用国际通用的拉丁字母，采用音素化的音节结构拼写以北京语音为标准音的普通话的一种方案。

# 字母表

| 字母 | 名称 |
|:---|:---|
| Aa | ㄚ |
| Bb | ㄅㄝ |
| Cc | ㄘㄝ | 
| Dd | ㄉㄝ |
| Ee | ㄜ | 
| Ff | ㄝㄈ | 
| Gg | ㄍㄝ | 
| Hh | ㄏㄚ |
| Ii | ㄧ |
| Jj | ㄐㄧㄝ |
| Kk | ㄎㄝ | 
| Ll | ㄝㄌ | 
| Mm | ㄝㄇ |
| Nn |ㄋㄝ  | 
| Oo | ㄛ |
| Pp | ㄆㄝ |
| Qq | ㄑㄧㄡ |
| Rr | ㄚㄦ |
| Ss | ㄝㄙ |
| Tt | ㄊㄝ |
| Uu | ㄨ |
| Vü | ㄪㄝ |
| Ww | ㄨㄚ |
| Xx | ㄒㄧ |
| Yy | ㄧㄚ |
| Zz | ㄗㄝ |

# 声母表

```
b
p
m
f
d
t
n
l
g
k
h
j
q
x
zh
ch
sh
r
z
c
s
y
w
```

# 韵母表

```
-iㄭzh(ẑ)、ch(ĉ)、sh(ŝ)、r、z、c、s单用时之韵母	
i ㄧ 衣
u ㄨ 乌
ü ㄩ 迂
a ㄚ 啊
ia ㄧㄚ 呀
ua ㄨㄚ 蛙
o ㄛ 喔
uo ㄨㄛ 窝
e ㄜ 鹅
ie ㄧㄝ 耶
yoㄧㄛ哟	
üe ㄩㄝ 约
ai ㄞ 哀
iaiㄧㄞ 厓	
uai ㄨㄞ 歪
ei ㄟ 诶
uei ㄨㄟ 威
ao ㄠ 熬
iao ㄧㄠ 腰
ou ㄡ 欧
iou ㄧㄡ 忧
an ㄢ 安
ian ㄧㄢ 烟
uɑn ㄨㄢ 弯
üan ㄩㄢ 冤
en ㄣ 恩
in ㄧㄣ 因
uen ㄨㄣ 温
ün ㄩㄣ 晕
ang ㄤ 昂
iang ㄧㄤ 央
uang ㄨㄤ 汪
eng ㄥ 亨的韵母;鞥
ing ㄧㄥ 英
ueng ㄨㄥ /u̯əŋ/翁
ong ㄨㄥ /ʊŋ/轰的韵母
iong ㄩㄥ 雍
êㄝ耶之韵母
```

(1) "知、蚩、诗、日、资、雌、思”等字的韵母用i。

(2) 韵母ㄦ写成er，用做韵尾的时候写成r。

(3 )韵母ㄝ单用的时候写成ê。

(4) i 行的韵母，前面没有声母的时候，写成yi（衣）， ya（呀）， ye（耶）， yao（腰），you（忧），yan（烟），yin（因），yanɡ（央），yinɡ（英），yonɡ（雍）。

u 行的韵母，前面没有声母的时候，写成wu（乌）， wa（蛙）， wo（窝）， wai（歪），wei（威），wan（弯），wen（温），wanɡ（汪），weng（翁）。

ü 行的韵母跟声母j,q,x拼的时候，写成ju（居），qu（区），xu（虚），ü上两点也省略；但是跟声母l,n拼的时候，仍然写成lü（吕），nü（女）。

(5) iou,uei,uen前面加声母的时候，写成iu,ui,un，例如niu（牛），gui（归），lun（论）。

# 声调

```
阴平  ˉ
阳平  ˊ
上声  ˇ
去声  ˋ
```

# 隔音符号

a，o，e开头的音节连接在其它音节后面的时候，如果音节的界限发生混淆，用隔音符号(`'`)隔开，例如pi'ao（皮袄）。

# 发音

平舌音(3个):zi ci si

翘舌音(4个):zhi chi shi ri

三拼音节：ia ua uo uai iao ian iang uang iong

零声母音节: a ai an ang ao e ê ei en eng er o ou

标调规则：有a别放过，没a找o、e，i、u并列标在后，这样标调准没错!

```
a：发音时，嘴唇自然张大，舌放平，舌头中间微隆，声带颤动。
o：发音时，嘴唇成圆形，微翘起，舌头向后缩，舌面后部隆起，舌居中，声带颤动。
e：发音时，嘴半开，舌位靠后，嘴角向两边展开成扁形，声带颤动。
i：发音时，嘴微张成扁平状，舌尖抵住下齿龈，舌面抬高，靠近上硬腭，声带颤动。
u：发音时，嘴唇拢圆，突出成小孔，舌面后部隆起，声带颤动。
ü：发音时，嘴唇成圆形，接近闭拢，舌尖抵住下齿龈，舌面前部隆起，声带颤动。
b：发音时，双唇紧闭，阻碍气流，然后双唇突然放开，让气流冲出，读音轻短。
p：发音时，双唇紧闭，阻碍气流，然后双唇突然放开，气流迸出成音。
m：发音时，双唇紧闭，舌后缩，气流从鼻腔出来，打开嘴，声带颤动。
f：发音时，上齿触下唇形成窄缝，让气流从缝中挤出来，摩擦成声。
d：发音时，舌尖抵住上牙床，憋住气流后突然放开，气流从口腔迸出，爆发成音。
t：发音时，舌尖抵住上牙床，憋住气后，突然离开，气流从口中迸出。
n：发音时，舌尖抵住上牙床，气流从鼻腔通过，同时冲开舌尖的阻碍，声带颤动。
l：发音时，嘴唇稍开，舌尖抵住上牙床，声带颤动，气流从舌尖两边流出。
g：发音时，舌根前部抵住软腭阻碍气流，让气流冲破舌根的阻碍，爆发成音。
k：发音时，舌根前部，抵住上软腭，阻碍气流，让气流冲破舌根的阻碍，迸发成音。
h：发音时，舌根抬高，接近软腭，形成窄缝，气流从缝中挤出，摩擦成音。
j：发音时，舌尖抵住下门齿，舌面前部紧贴硬腭，气流从窄缝中冲出，摩擦成音。
q：发音时，舌面前部贴住硬腭，气流冲破舌根的阻碍，摩擦成音。
x：发音时，舌尖抵住下门齿，舌面前部抬高靠近硬腭，形成窄缝，气流从缝中挤出，摩擦成音。
zh：发音时，舌尖上翘，抵住硬腭前部，有较弱的气流冲开舌尖阻碍，从缝中挤出，摩擦成音。
ch：发音时，舌尖上翘，抵住硬腭前部，有较强的气流冲开舌尖阻碍，从缝中挤出，摩擦成音。
sh：发音时，舌尖上翘，靠近硬腭前部，留出窄缝，气流从窄缝中挤出，摩擦成音。
r：发音时，舌尖上翘，靠近硬腭前部，留出窄缝，嗓子用力发音，气流从窄缝中挤出，摩擦成音，声带颤动。
z：发音时，舌尖抵住上门齿背，阻碍气流，让较弱的气流冲开舌尖阻碍，从窄缝中挤出，摩擦音。
c：发音时，舌尖抵住上门齿背，阻碍气流，让较强的气流从缝中挤出，摩擦成音。
s：发音时，舌尖接近上门齿背，留出窄缝，气流从舌尖的窄缝中挤出，摩擦成音。
y：发音时，嘴微张成扁平状，舌尖抵住下齿龈，舌面抬高，靠近上硬腭，声带颤动。
w：发音时，嘴唇拢圆，突出成小孔，舌面后部隆起，声带颤动。
ai：发音时，先发 a 的音，然后滑向i，气流不中断，读音轻短。
ei：发音时，先发 e 的音，然后滑向i，气流不中断，嘴角向两边展开。
ui：发音时，u 的发音轻短，然后滑向ei，嘴形由圆到扁。
ao：发音时，先发 a 的音，然后舌尖后缩，舌根向上抬，嘴形拢成圆形，轻轻的滑向 o。
ou：发音时，先发 o 的音，嘴唇渐收拢，舌根抬高，口型由大圆到小圆。
iu：发音时，先发 i，然后向ou滑动，口型由扁到圆。
ie：发音时，先发 i，再发e，气流不中断。
üe：发音时，先发 ü 的音，然后向e滑动，口型由圆到扁。
er：发音时，舌位居中发 e 的音，然后舌尖向硬腭卷起，两个字母同时发音。
an：发音时，先发 a 的音，然后舌尖逐渐抬起，顶住上牙床发n的音。
en：发音时，先发 e 的音，然后舌面抬高,舌尖抵住上牙床，气流从鼻腔泄出，发n的音。
in：发音时，先发 i 的音，然后舌尖抵住下门齿背，舌面渐至硬腭，气流从鼻腔泄出，发en的音。
un：发音时，先发 u 的音，然后舌尖抵住上牙床，接着发en的音，气流从鼻腔泄出。
ün：发音时，先发 ü 的音，然后舌头上抬，抵住上牙床，气流从鼻腔泄出，发en的音。
ang：发音时，先发 a 的音，然后舌根抵住上软腭，气流从鼻腔泄出，发后鼻音尾ng的音。
eng：发音时，先发 e 的音，然后舌尖抵住下牙床，舌根后缩抵住软腭发ng音，气流从鼻腔泄出。
ing：发音时，舌尖触下齿龈，舌面隆起至硬腭，鼻腔共鸣成声。
ong：发音时，先发 o 的音，然后舌根后缩抵住软腭，舌面隆起，嘴唇拢圆，鼻腔共鸣成声。
```

## 注意事项

拼写需注意的事项：

1. j、q、x、y遇到ü ，两个小点要拿去

2. 句子开头的首字母要大写;汉语人名的开头字母要大写;专有名词的开头字母要大写例：Beijing;文章标题开头字母要大写。

# 参考资料

[百度百科-汉语拼音字母](https://baike.baidu.com/item/%E6%B1%89%E8%AF%AD%E6%8B%BC%E9%9F%B3%E5%AD%97%E6%AF%8D/1884486?fr=aladdin)

* any list
{:toc}