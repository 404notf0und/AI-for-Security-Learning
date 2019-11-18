本篇文章主要结合自己的亲身经历和体会表达一下对AI for Security的看法，整体态度偏消极。
## 0x01 背景 ##
本段将由大到小从国家、网上公开资料、项目三个方面说明智能化安全对抗时代的来临。
正如有时候觉得学得好不如嫁得好，在网络安全方面有时也是学得好不如运气好跟上了历史的进程。网络战早已被美军纳入作战体系，现如今中美关系对抗愈加激烈，随之而来的可能是成规模的网络对抗，从当前看来，AI技术比较适合大幅度提升网络对抗能力，所以智能化的网络对抗技术可能得到国家级的重点推进。笔者跟踪了几年来网上关于智能化安全的一些研究和进展，发现几年前大家重点研究的是AI安全检测，仅仅是弱智能化的安全防护，远达不到对抗的烈度，现如今随着对抗样本等对抗技术的火热，智能化安全对抗越来越得到学术界研究者的关注，无论是算法领域研究者，还是安全领域研究者。按照时间线，我经历的几个项目主题分别是：防御、反制、进攻、对抗，对抗烈度明显增加，这也许正验证着开头分析过的国家面临的安全对抗问题，相较于传统对抗手段，智能化的安全对抗技术显得不可或缺。

## 0x02 智能化安全对抗 ##
AI和安全之间的关系可分为四点：
- 应用安全
	- 用AI来做应用安全防护
	- 用AI来攻击应用
- AI本身安全
	- (用AI)攻击AI(模型、系统、框架)
	- AI模型防护

AI是手段，目标是安全，包括应用安全和AI安全。所以是AI for Application and AI Security，即AI for Security。

从应用安全的角度来说，用AI来做应用安全防护，比如做WAF或入侵检测，属于基础安全，做反欺诈检测，属于业务安全；用AI来攻击应用，比如用AI来自动化漏洞挖掘，属于系统安全，用AI来攻击验证码，属于业务安全；而从AI本身安全来说，(用AI)攻击AI，比如用对抗样本攻击AI模型，属于AI模型安全，用数据污染的手段攻击AI模型，属于AI数据安全；AI模型防护，比如对抗对抗样本和对抗数据污染，比较小众。

四者相辅相成，假如我们在防守位，正遭遇外界的攻击，包括传统攻击和AI攻击，如果我们用AI来做应用安全防护，对手可能采用对抗样本来攻击我们的AI，那么我们就要对AI模型进行防护，也就是对抗对抗样本。假如我们在攻击位，之前的过程颠倒即可。总的来说，攻防就是一个动态博弈的过程。

## 0x03 学术界和工业界前沿智能化安全对抗 ##
学术界研究者近几年比较关注对抗样本等智能化对抗技术，在四大顶会上也不断发表了系列关于机器学习和安全对抗的文章，有传统的机器学习安全检测文章，也有机器学习模型本身安全性对抗的文章，比如11月28日在湖北武汉举办的第八届全国网络与信息安全防护峰会(XDef2018安全峰会)第二天的议题中，来自中科院信工所和浙江大学的两位博士生展示了他们的研究成果：“恶魔音乐”攻击智能语音系统和DEEPSEC：面向深度学习模型的安全性评估系统，两项成果都是关于机器学习的安全对抗，分别发表在全球四大安全顶会中的Usenix Security 2018和IEEE S&P 2019，代表着学术界最新的研究进展。可以看出学术界的研究点开始转向了关于机器学习的对抗性技术研究。前几天去参加的XDef2018会议，对阿里巴巴集团安全部资深算法专家周涛博士分享的议题《机器学习还是统计模型：大数据安全分析应用实战》很感兴趣，可能代表着工业界对AI for Security的理解和做法，可能由于需求导致出发点不同，该议题重点在于防：AI安全检测和抵抗机器学习流量。AI作为一种手段，可以降维打击传统攻击，抵抗同级的AI攻击，但是要在实际场景中大规模应用还需要做大量工作，现在AI还只是弱智能化，适合加以利用做辅助决策。分享的内容都是主流的做法，所以我想工业界最新的成果大多不会公开，现在随着学术流高学历人才不断加入互联网公司，从而学术工程化，所以工业界的实力也应该是天花板。这就可能造成一个问题，我们容易得到并且消化的智能化安全对抗技术的资料都是价值过剩的资料。比如学术界研究的智能化对抗性技术都是偏研究性质的论文，实际的工程化可能较难，并且学术界可能也不会太关注工程化，对许多人来说，要吸收学术界前沿知识的门槛很高，对于大公司的尖端人才来说，可能再加以研究再工程化，成果当然不会公开。所以对于一般人来说，很难获取一手的学术界和工业界的智能化对抗技术，并且很难做到前沿技术工程化。

我们现在容易获取的资料主要集中在是AI安全检测方面，大部分文章都在自娱自乐，反反复复换汤不换药，都是同样的套路，未加以优化，质量低，只适合做做实验，很少在实际的生产环境下测试，效果未加以验证。

## 0x04 我的AI for Security 学习笔记 ##
针对上面分析到的问题，我筛选整理了一份安全场景、基于AI的安全算法和安全数据分析学习资料，希望对AI for Security感兴趣的朋友们有所帮助。

# AI-for-Security-Learning
安全场景、基于AI的安全算法和安全数据分析学习笔记（工程类学习笔记，不包含论文、书籍、视频等，不花里胡哨嘻嘻哈哈）

项目地址：https://github.com/404notf0und/AI-for-Security-Learning

最近更新日期为：2018/12/2

同步更新于：[404 Not Found：AI for Security](http://www.4o4notfound.org)

目录：
- [防护篇](#防护篇)
	- [使用AI保护应用](#使用AI保护应用)
		- [恶意软件和代码](#恶意软件和代码)
		- [恶意流量检测](#恶意流量检测)
		- [域名安全检测](#域名安全)
		- [业务安全检测](#业务安全)
		- [Web安全检测](#Web安全)
			- [URL异常检测](#Web安全之URL异常检测)
			- [XSS检测](#Web安全之XSS检测)
			- [Web攻击多分类检测](#Web安全之攻击多分类检测)
			- [Webshell检测](#Web安全之Webshell检测)
			- [Other](#Web安全之其他)
		- [杂项](#杂项)
			- WindowsRDP检测
			- PowerShell检测
			- 用户行为(UBA)检测
			- 弱口令检测
			- 安全运营
	- [(使用AI)保护AI(框架、数据、模型、系统)](#保护AI)
- [对抗篇](#对抗篇)
	- [使用AI攻击应用](#使用AI攻击应用)
	- [(使用AI)攻击AI(框架、数据、模型、系统)](#攻击AI)
		- [攻击AI框架](#攻击AI框架)
		- [攻击AI模型](#攻击AI模型)
<!-- more -->

# 防护篇 #
## 使用AI保护应用 ##
### 恶意软件和代码 ###
- [深度学习在恶意软件检测中的应用](https://xz.aliyun.com/t/2447)
- [恶意软件与数据分析](https://iami.xyz/AliSEC3/)
- [利用机器学习进行恶意代码分类](http://drops.xmd5.com/static/drops/tips-8151.html)
- [用机器学习检测Android恶意代码](http://drops.xmd5.com/static/drops/mobile-13428.html)
- [Malware Detection in Executables Using Neural Networks](https://devblogs.nvidia.com/malware-detection-neural-networks/)
- [基于深度学习的恶意样本行为检测(含源码)](https://www.freebuf.com/articles/system/182566.html)

### 恶意流量检测 ###
- [利用机器学习检测HTTP恶意外连流量](https://www.freebuf.com/column/170483.html)

### 域名安全检测 ###
- [使用fasttext进行DGA检测](https://iami.xyz/DGA-Detect/)
- [使用CNN检测DNS隧道](https://github.com/BoneLee/dns_tunnel_dectect_with_CNN)
- [机器学习与威胁情报的融合：一种基于AI检测恶意域名的方法](https://www.freebuf.com/articles/es/187451.html)

### 业务安全检测 ###
- [基于设备指纹的风控建模以及机器学习的尝试](https://xz.aliyun.com/t/2801)
- [如何在安全风控中评估和量化机器学习有效性](https://xz.aliyun.com/t/2951)
- [人工智能反欺诈三部曲——特征工程](https://www.anquanke.com/post/id/85741)

### Web安全检测 ###
### Web安全之URL异常检测 ###
- [基于机器学习的web异常检测](https://www.freebuf.com/articles/web/126543.html)
- [基于大数据和机器学习的Web异常参数检测系统Demo实现](https://www.freebuf.com/articles/web/134334.html)
- [基于机器学习的web应用防火墙](https://github.com/faizann24/Fwaf-Machine-Learning-driven-Web-Application-Firewall)
- [LSTM识别恶意HTTP请求](https://www.cdxy.me/?p=775)
- [基于URL异常检测的机器学习模型mini部署](http://4o4notfound.org/index.php/archives/84/)
- [我的AI安全检测学习笔记（一）](http://4o4notfound.org/index.php/archives/127/)

### Web安全之XSS检测 ###
- [机器学习识别XSS实践](https://www.cdxy.me/?p=773)
- [使用深度学习检测XSS](http://webber.tech/posts/%E4%BD%BF%E7%94%A8%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E6%A3%80%E6%B5%8BXSS/)
- [使用深度学习检测XSS(续)](http://webber.tech/posts/%E4%BD%BF%E7%94%A8%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E6%A3%80%E6%B5%8BXSS%28%E7%BB%AD%29/)

### Web安全之攻击多分类检测 ###
- [基于机器学习的WEB攻击分类检测模型](https://www.freebuf.com/news/184687.html)
- [基于机器学习的攻击检测系统](https://www.freebuf.com/column/189981.html)

### Web安全之Webshell检测 ###
- [基于机器学习的分布式webshell检测系统-特征工程（1）](https://www.s0nnet.com/archives/fshell-feature-1)
- [深度学习PHP webshell查杀引擎demo](https://www.cdxy.me/?p=788)
- [使用机器学习识别WebShell](https://github.com/lcatro/WebShell-Detect-By-Machine-Learning)
- [基于机器学习的分布式Webshell检测系统](https://github.com/Lingerhk/fshell)
- [GitChat · 安全 | 基于机器学习的 Webshell 发现技术探索](http://blog.csdn.net/GitChat/article/details/77932384?locationNum=4&fps=1)
- [刘焱： Webshell 发现技术实战解析](http://gitbook.cn/books/5964d154cc597d3e0c08667c/index.html)
- [安普诺张涛：再谈webshell检测](http://www.cnetsec.com/article/22593.html)
- [新开始:webshell的检测](https://iami.xyz/New-Begin-For-Nothing/)
- [基于机器学习的WebShell检测方法与实现(上)](https://www.freebuf.com/articles/web/181169.html)

### Web安全之其他 ###
- [Web安全检测中机器学习的经验之谈](https://iami.xyz/ML-IN-Webshell-Detection-Advantages-And-Disadvantages/)

### 杂项 ###
- [机器学习在WindowsRDP版本和后门检测上的应用](https://www.anquanke.com/post/id/157175)
- [用机器学习检测恶意PowerShell](https://xz.aliyun.com/t/2437)
- [机器学习算法在用户行为检测(UBA)领域的应用](http://dearcharles.cn/2017/11/11/%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%E7%AE%97%E6%B3%95%E5%9C%A8%E7%94%A8%E6%88%B7%E8%A1%8C%E4%B8%BA%E6%A3%80%E6%B5%8B-UBA-%E9%A2%86%E5%9F%9F%E7%9A%84%E5%BA%94%E7%94%A8/)
- [利用机器学习和规则实现弱口令检测](https://manning23.github.io/2018/10/12/%E5%88%A9%E7%94%A8%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%E5%92%8C%E8%A7%84%E5%88%99%E5%AE%9E%E7%8E%B0%E5%BC%B1%E5%8F%A3%E4%BB%A4%E6%A3%80%E6%B5%8B/)
- [解决机器学习和安全运营之间的最后一公里问题](https://www.anquanke.com/post/id/163637)

## 保护AI ##
- [如何利用AI对抗“数据污染”和”数据中毒“？](https://www.anquanke.com/post/id/150653)
- [对抗数据中毒--机器学习在阿里巴巴网络安全的应用](https://www.leiphone.com/news/201806/rYrfwtaeCNohEf0D.html)

# 对抗篇 #
## 使用AI攻击应用 ##
- [AI与Android漏洞挖掘的那些事儿](https://www.zybuluo.com/qinyun/note/957067)
- [AI与安全的恩怨情仇五部曲「1」Misuse AI](https://www.zuozuovera.com/archives/1565/)
- [一种基于机器学习的自动化鱼叉式网络钓鱼思路](https://www.freebuf.com/articles/web/132811.html)

## 攻击AI ##
### 攻击AI框架 ###
- [深度学习框架中的魔鬼——探究人工智能系统中的安全问题](https://www.anquanke.com/post/id/86989)

### 攻击AI模型 ###
- [安全领域中机器学习的对抗和博弈](http://bindog.github.io/blog/2016/11/13/game-playing-with-ml-in-security/)
- [基础攻防场景下的AI对抗样本初探](https://www.cdxy.me/?p=798)
- [机器学习在安全攻防场景的应用与分析](https://www.freebuf.com/articles/neopoints/152457.html)
- [使用生成对抗网络(GAN)生成DGA](http://webber.tech/posts/%E4%BD%BF%E7%94%A8%E7%94%9F%E6%88%90%E5%AF%B9%E6%8A%97%E7%BD%91%E7%BB%9C%28GAN%29%E7%94%9F%E6%88%90DGA/)
- [详解如何使用Keras实现Wassertein GAN](https://mp.weixin.qq.com/s/F2gBP23LCEF72QDlugbBZQ)
- [Is attacking machine learning easier than defending it?](http://www.cleverhans.io/security/privacy/ml/2017/02/15/why-attacking-machine-learning-is-easier-than-defending-it.html)
- [对深度学习的逃逸攻击 ——探究人工智能系统中的安全盲区](https://www.anquanke.com/post/id/87037)

## 0x05 对现状的个人理解 ##
从上面我收集的资料来看，目前易工程化的还主要集中在AI安全检测方面，但是大规模应用还是较难，还存在相当多的问题，尤其是深度学习。从场景来说，安全领域的场景非常复杂，各不相同，想找到通用的方法论解决所有问题怕是天方夜谭，所以需要对每种小场景结合机器学习技术具体处理，这就涉及到大量的人力财力和物力；从数据来说，就算不牵扯复杂的安全场景，安全数据的同构化也是一项挑战，李飞飞教授（是犹他大学的李飞飞，好像现在在阿里，不是斯坦福的李飞飞）发表在CCS的研究成果：DeepLog，可以解决这个问题；从模型来看，不考虑模型效果，机器学习和深度学习训练的模型的可解释性还是较弱，学术界已经开始尝试突破深度学习的可解释性问题，希望可以看见曙光。总的来说，连目前相对容易做的AI安全检测大规模应用都还存在问题，更何况智能化安全对抗技术了，但是形势不等人啊，智能化安全对抗已经来了，然而技术还没准备好。也许是因为在同一个环境太久，接触到的资源比较局限，所以限制了自己的视野，所以希望年后能找实习历练一下，让机器学习真正的在安全场景中落地。

## 0x06 Reference ##
Machine Learning Blog:

https://plushunter.github.io

http://phoebepan.cn

http://scarletpan.github.io

http://www.jeyzhang.com

Machine Learning+Security Blog:

http://webber.tech/

http://bindog.github.io

https://www.cdxy.me

https://iami.xyz

https://www.zuozuovera.com/

https://www.cnblogs.com/LittleHann
