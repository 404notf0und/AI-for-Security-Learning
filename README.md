# AI-for-Security-Learning
安全场景、基于AI的安全算法和安全数据分析学习笔记（偏工程类学习笔记），持续阅读，保持对业界技术的跟进和迭代

项目地址：https://github.com/404notf0und/AI-for-Security-Learning

最近更新日期为：2020/02/12

新增：
- [CNN+BLSTM+CTC的验证码识别从训练到部署](https://mp.weixin.qq.com/s/2v86piOgtK_t--Pzu28LgQ)
- [DNS Tunnel隧道隐蔽通信实验 && 尝试复现特征向量化思维方式检测](https://www.cnblogs.com/LittleHann/p/8656621.html)
- [第三届阿里云安全赛季军-0day](https://zhuanlan.zhihu.com/p/77492583)
- [第三届阿里云安全算法挑战赛冠军代码](https://github.com/poteman/Alibaba-3rd-Security-Algorithm-Challenge)
- [**基于机器学习的恶意软件加密流量检测研究分享**](https://blog.riskivy.com/%e5%9f%ba%e4%ba%8e%e6%9c%ba%e5%99%a8%e5%ad%a6%e4%b9%a0%e7%9a%84%e6%81%b6%e6%84%8f%e8%bd%af%e4%bb%b6%e5%8a%a0%e5%af%86%e6%b5%81%e9%87%8f%e6%a3%80%e6%b5%8b/?from=groupmessage&isappinstalled=0)
- [**探秘-基于机器学习的DNS隐蔽隧道检测方法与实现**](https://blog.riskivy.com/%e6%8e%a2%e7%a7%98-%e5%9f%ba%e4%ba%8e%e6%9c%ba%e5%99%a8%e5%ad%a6%e4%b9%a0%e7%9a%84dns%e9%9a%90%e8%94%bd%e9%9a%a7%e9%81%93%e6%a3%80%e6%b5%8b%e6%96%b9%e6%b3%95%e4%b8%8e%e5%ae%9e%e7%8e%b0/)
- [**AI繁荣下的隐忧——Google Tensorflow安全风险剖析**](https://security.tencent.com/index.php/blog/msg/130)
- [**污染TensorFlow模型: XCTF 2019 Final tfboys命题思路**](https://www.cdxy.me/?p=813)
- [**使用TextCNN模型探究恶意软件检测问题**](https://xz.aliyun.com/t/6785)
- [**基于卷积神经网络的恶意代码家族标注**](https://xz.aliyun.com/t/6705)
- [**Deep learning rises: New methods for detecting malicious PowerShell**](https://www.microsoft.com/security/blog/2019/09/03/deep-learning-rises-new-methods-for-detecting-malicious-powershell/)
- [**使用生成对抗网络(GAN)生成DGA**](http://webber.tech/posts/%E4%BD%BF%E7%94%A8%E7%94%9F%E6%88%90%E5%AF%B9%E6%8A%97%E7%BD%91%E7%BB%9C%28GAN%29%E7%94%9F%E6%88%90DGA/)
- [**机器学习在二进制代码相似性分析中的应用**](https://mp.weixin.qq.com/s?__biz=MjM5NTc2MDYxMw==&mid=2458303210&idx=1&sn=345f8cec156ada8fa9bf6a6d6de83906&chksm=b1818a6086f60376e766baf472171d8e2c780b2913568b46b683e3112fcc5f86c9bf4c19e38b&mpshare=1&scene=1&srcid=&sharer_sharetime=1580984631757&sharer_shareid=5dc01f49f38fd64ff3e64844bc7d2ea7&exportkey=A0qHBeUryuXO6zhGWt5OJNw%3D&pass_ticket=gjTFXl4hPMTBWzlKpWZWqK8HivXQ8q7ChNndmw4I8JrdAK0jWWFvKIq7OMnO3BhL#rd)

同步更新于：[404 Not Found：AI for Security](http://4o4notfound.org/index.php/archives/177/)

目录：
- [综述篇](#综述篇)
- [防护篇](#防护篇)
	- [使用AI保护应用](#使用AI保护应用)
		- [恶意样本检测](#恶意样本检测)
		- [入侵检测](#入侵检测)
		- [域名安全检测](#域名安全检测)
		- [业务安全检测](#业务安全检测)
		- [Web安全检测](#Web安全检测)
			- [URL异常检测](#Web安全之URL异常检测)
			- [SQLi检测](#Web安全之SQLi检测)
			- [XSS检测](#Web安全之XSS检测)
			- [Web攻击多分类检测](#Web安全之攻击多分类检测)
			- [Webshell检测](#Web安全之Webshell检测)
			- [Other](#Web安全之其他)
		- [APT检测](#APT检测)
		- [安全运营](#安全运营)
		- [二进制安全](#二进制安全)
		- [杂项](#杂项)
			- WindowsRDP检测
			- PowerShell检测
			- 用户行为(UBA)检测
			- 弱口令检测
	- [(使用AI)保护AI(框架、数据、模型、系统)](#保护AI)
- [对抗篇](#对抗篇)
	- [使用AI攻击应用](#使用AI攻击应用)
	- [(使用AI)攻击AI(框架、数据、模型、系统)](#攻击AI)
		- [攻击AI框架](#攻击AI框架)
		- [攻击AI模型](#攻击AI模型)
- [心得体会篇](#心得体会篇)
- [学习交流篇](#学习交流篇)
<!-- more -->

# 综述篇 #
- [安全智能应用的一些迷思](https://zhuanlan.zhihu.com/p/88042567)
- [深度总结 | 机器智能的安全之困](https://mp.weixin.qq.com/s?__biz=MzU5ODUxNzEyNA==&mid=2247484911&idx=1&sn=6a7cc2268dda2aab38085c555c04b209&chksm=fe43b104c934381294eba27b1385bffbfaf9c984773eba4cf489f26357afb50f19b382c6b500&mpshare=1&scene=1&srcid=&sharer_sharetime=1571808765043&sharer_shareid=5dc01f49f38fd64ff3e64844bc7d2ea7&key=bad1bd95c2b983fbcd2131a6fe96a7eeee59983a46ca6da6917131030413a4871bd05d4f62253d3680caf742fedcc2273637369cd4b3193eea2832db38b59be8aa0f01f4c9526a8e0c14a2805d252e95&ascene=1&uin=MTA5NjU5ODIxNg%3D%3D&devicetype=Windows+7&version=6207014a&lang=zh_CN&pass_ticket=LGfguXV%2FO1DU8mbAUL8nHSOLBI0LcXBegrVpx%2FcaDZi0HZOJ1h6pp23xChmPHqPu)
# 防护篇 #
## 使用AI保护应用 ##
### 恶意样本检测 ###
- [深度学习在恶意软件检测中的应用](https://xz.aliyun.com/t/2447)
- [恶意软件与数据分析](https://iami.xyz/AliSEC3/)
- [利用机器学习进行恶意代码分类](http://drops.xmd5.com/static/drops/tips-8151.html)
- [用机器学习检测Android恶意代码](http://drops.xmd5.com/static/drops/mobile-13428.html)
- [Malware Detection in Executables Using Neural Networks](https://devblogs.nvidia.com/malware-detection-neural-networks/)
- [基于深度学习的恶意样本行为检测(含源码)](https://www.freebuf.com/articles/system/182566.html)
- [用机器学习进行恶意软件检测——以阿里云恶意软件检测比赛为例](https://xz.aliyun.com/t/3704)
- [第二届微软恶意软件预测挑战赛初探](http://4o4notfound.org/index.php/archives/179/)
- [DataCon大数据安全分析比赛冠军思路分享：方向二-恶意代码检测](https://zhuanlan.zhihu.com/p/64252076)
- [第三届阿里云安全赛季军-0day](https://zhuanlan.zhihu.com/p/77492583)
- [第三届阿里云安全算法挑战赛冠军代码](https://github.com/poteman/Alibaba-3rd-Security-Algorithm-Challenge)
- [使用TextCNN模型探究恶意软件检测问题](https://xz.aliyun.com/t/6785)
- [基于卷积神经网络的恶意代码家族标注](https://xz.aliyun.com/t/6705)

### 入侵检测 ###
- [利用机器学习检测HTTP恶意外连流量](https://www.freebuf.com/column/170483.html)
- [ExecScent: Mining for New C&C Domains in Live
Networks with Adaptive Control Protocol Templates](https://www.usenix.org/system/files/conference/usenixsecurity13/sec13-paper_nelms.pdf)
- [MADE: Security Analytics for Enterprise Threat Detection](http://www.ccs.neu.edu/home/alina/papers/MADE.pdf)
- [机器学习在互联网巨头公司实践](https://mp.weixin.qq.com/s/NFqUF824Rpr4g6wYWFpSNQ)
- [机器学习在入侵检测方面的应用 - 基于ADFA-LD训练集训练入侵检测判别模型](https://www.cnblogs.com/LittleHann/p/7806093.html#_lab2_0_1)
- [datacon比赛方向三-攻击源与攻击者分析writeup](https://github.com/ReAbout/datacon)
- [基于机器学习的恶意软件加密流量检测研究分享](https://blog.riskivy.com/%e5%9f%ba%e4%ba%8e%e6%9c%ba%e5%99%a8%e5%ad%a6%e4%b9%a0%e7%9a%84%e6%81%b6%e6%84%8f%e8%bd%af%e4%bb%b6%e5%8a%a0%e5%af%86%e6%b5%81%e9%87%8f%e6%a3%80%e6%b5%8b/?from=groupmessage&isappinstalled=0)
- [anomaly-detection-through-reinforcement-learning](https://zighra.com/blogs/anomaly-detection-through-reinforcement-learning/)

### 域名安全检测 ###
- [机器学习与威胁情报的融合：一种基于AI检测恶意域名的方法](https://www.freebuf.com/articles/es/187451.html)
- [使用fasttext进行DGA检测](https://iami.xyz/DGA-Detect/)
- [机器学习实践-DGA检测](http://galaxylab.org/%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%E5%AE%9E%E8%B7%B5-dga%E6%A3%80%E6%B5%8B/)
- [使用生成对抗网络(GAN)生成DGA](http://webber.tech/posts/%E4%BD%BF%E7%94%A8%E7%94%9F%E6%88%90%E5%AF%B9%E6%8A%97%E7%BD%91%E7%BB%9C%28GAN%29%E7%94%9F%E6%88%90DGA/)
- [使用CNN检测DNS隧道](https://github.com/BoneLee/dns_tunnel_dectect_with_CNN)
- [DNS Tunnel隧道隐蔽通信实验 && 尝试复现特征向量化思维方式检测](https://www.cnblogs.com/LittleHann/p/8656621.html)
- [探秘-基于机器学习的DNS隐蔽隧道检测方法与实现](https://blog.riskivy.com/%e6%8e%a2%e7%a7%98-%e5%9f%ba%e4%ba%8e%e6%9c%ba%e5%99%a8%e5%ad%a6%e4%b9%a0%e7%9a%84dns%e9%9a%90%e8%94%bd%e9%9a%a7%e9%81%93%e6%a3%80%e6%b5%8b%e6%96%b9%e6%b3%95%e4%b8%8e%e5%ae%9e%e7%8e%b0/)
- [DataCon 2019: 1st place solution of malicious DNS traffic & DGA analysis](https://www.cdxy.me/?p=806)
- [DataCon 9102: DNS Analysis](https://github.com/shyoshyo/Datacon-9102-DNS)
- [Datacon DNS攻击流量识别 内测笔记](http://momomoxiaoxi.com/数据分析/2019/04/24/datacondns1/)

### 业务安全检测 ###
- [基于设备指纹的风控建模以及机器学习的尝试](https://xz.aliyun.com/t/2801)
- [如何在安全风控中评估和量化机器学习有效性](https://xz.aliyun.com/t/2951)
- [阿里巴巴直播内容风险防控中的AI力量](https://zhuanlan.zhihu.com/p/24690287)
- [人工智能反欺诈三部曲——特征工程](https://www.anquanke.com/post/id/85741)
- [人工智能反欺诈三部曲之：设备指纹](https://zhuanlan.zhihu.com/p/31712434)

### Web安全检测 ###
### Web安全之URL异常检测 ###
- [基于机器学习的web异常检测](https://www.freebuf.com/articles/web/126543.html)
- [基于大数据和机器学习的Web异常参数检测系统Demo实现](https://www.freebuf.com/articles/web/134334.html)
- [基于机器学习的web应用防火墙](https://github.com/faizann24/Fwaf-Machine-Learning-driven-Web-Application-Firewall)
- [LSTM识别恶意HTTP请求](https://www.cdxy.me/?p=775)
- [基于URL异常检测的机器学习模型mini部署](http://4o4notfound.org/index.php/archives/84/)
- [我的AI安全检测学习笔记（一）](http://4o4notfound.org/index.php/archives/127/)
- [A Deep Learning Based Online Malicious URL and DNS Detection Scheme](https://link.springer.com/chapter/10.1007/978-3-319-78813-5_22)
- [POSTER: A PU Learning based System for Potential Malicious URL Detection](https://dl.acm.org/citation.cfm?id=3138825)

### Web安全之SQLi检测
- [三种特征向量对深度学习攻击检测的影响](https://manning23.github.io/2017/08/08/三种特征向量对深度学习攻击检测的影响/)

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
- [基于机器学习的Webshell发现技术探索](https://mp.weixin.qq.com/s/1V0xcjH-6V5qJoJILP0pJQ)
- [刘焱： Webshell 发现技术实战解析](http://gitbook.cn/books/5964d154cc597d3e0c08667c/index.html)
- [安普诺张涛：再谈webshell检测](http://www.cnetsec.com/article/22593.html)
- [新开始:webshell的检测](https://iami.xyz/New-Begin-For-Nothing/)
- [基于机器学习的WebShell检测方法与实现(上)](https://www.freebuf.com/articles/web/181169.html)
- [初探机器学习检测PHP Webshell](https://paper.seebug.org/526/)

### Web安全之其他 ###
- [Web安全检测中机器学习的经验之谈](https://iami.xyz/ML-IN-Webshell-Detection-Advantages-And-Disadvantages/)

### APT检测
- [APT detection based on machine learning](https://mp.weixin.qq.com/s?__biz=MzU5MTM5MTQ2MA==&mid=2247484139&idx=1&sn=0da63a49f341eccc0bb48c954d8ebbb4&chksm=fe2efd60c95974767521fe6a6b7257a1d05e5482fc7ddeda281bdf0f0deb20add82d1a82d8ec&mpshare=1&scene=1&srcid=&pass_ticket=bjnNiDKomd79pQvRonW%2BXsTe6JrO%2FFs6oII12dZaLBPuQOtNK6Rzh9WSJ%2B%2F89ZUA#rd)
- [RSAC 2019 | 机器学习算法分析引擎助力安全威胁推理分析](http://blog.nsfocus.net/machine-learning-algorithms-analysis-engine-security-threat-reasoning/)

### 安全运营
- [解决机器学习和安全运营之间的最后一公里问题](https://www.anquanke.com/post/id/163637)
- [Data-Knowledge-Action: 企业安全数据分析入门](https://www.cdxy.me/?p=803)
- [RSAC 2019 | 采用NLP机器学习来进行自动化合规风险治理](http://blog.nsfocus.net/automated-compliance-risk-management-nlp-machine-learning/)

### 二进制安全
- [机器学习在二进制代码相似性分析中的应用](https://mp.weixin.qq.com/s?__biz=MjM5NTc2MDYxMw==&mid=2458303210&idx=1&sn=345f8cec156ada8fa9bf6a6d6de83906&chksm=b1818a6086f60376e766baf472171d8e2c780b2913568b46b683e3112fcc5f86c9bf4c19e38b&mpshare=1&scene=1&srcid=&sharer_sharetime=1580984631757&sharer_shareid=5dc01f49f38fd64ff3e64844bc7d2ea7&exportkey=A0qHBeUryuXO6zhGWt5OJNw%3D&pass_ticket=gjTFXl4hPMTBWzlKpWZWqK8HivXQ8q7ChNndmw4I8JrdAK0jWWFvKIq7OMnO3BhL#rd)

### 杂项 ###
- [机器学习在WindowsRDP版本和后门检测上的应用](https://www.anquanke.com/post/id/157175)
- [用机器学习检测恶意PowerShell](https://xz.aliyun.com/t/2437)
- [Deep learning rises: New methods for detecting malicious PowerShell](https://www.microsoft.com/security/blog/2019/09/03/deep-learning-rises-new-methods-for-detecting-malicious-powershell/)
- [机器学习算法在用户行为检测(UBA)领域的应用](http://dearcharles.cn/2017/11/11/%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%E7%AE%97%E6%B3%95%E5%9C%A8%E7%94%A8%E6%88%B7%E8%A1%8C%E4%B8%BA%E6%A3%80%E6%B5%8B-UBA-%E9%A2%86%E5%9F%9F%E7%9A%84%E5%BA%94%E7%94%A8/)
- [利用机器学习和规则实现弱口令检测](https://manning23.github.io/2018/10/12/%E5%88%A9%E7%94%A8%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%E5%92%8C%E8%A7%84%E5%88%99%E5%AE%9E%E7%8E%B0%E5%BC%B1%E5%8F%A3%E4%BB%A4%E6%A3%80%E6%B5%8B/)
- [一个关于人工智能渗透测试分析系列](https://github.com/hongriSec/AI-Machine-Learning-Security)
- [机器学习在安全攻防场景的应用与分析](https://www.freebuf.com/articles/neopoints/152457.html)

## 保护AI ##
- [如何利用AI对抗“数据污染”和”数据中毒“？](https://www.anquanke.com/post/id/150653)
- [对抗数据中毒--机器学习在阿里巴巴网络安全的应用](https://www.leiphone.com/news/201806/rYrfwtaeCNohEf0D.html)

# 对抗篇 #
## 使用AI攻击应用 ##
- [AI与Android漏洞挖掘的那些事儿](https://www.zybuluo.com/qinyun/note/957067)
- [AI与安全的恩怨情仇五部曲「1」Misuse AI](https://www.zuozuovera.com/archives/1565/)
- [一种基于机器学习的自动化鱼叉式网络钓鱼思路](https://www.freebuf.com/articles/web/132811.html)
- [Weaponizing data science for social engineering:
Automated E2E spear phishing on Twitter](https://www.blackhat.com/docs/us-16/materials/us-16-Seymour-Tully-Weaponizing-Data-Science-For-Social-Engineering-Automated-E2E-Spear-Phishing-On-Twitter-wp.pdf)
- [Deep Exploit: Fully automatic penetration test tool using Machine Learning](https://securityonline.info/deep-exploit/)
- [GyoiThon: Fully automatic penetration test tool using Machine Learning](https://github.com/gyoisamurai/GyoiThon)
- [CNN+BLSTM+CTC的验证码识别从训练到部署](https://mp.weixin.qq.com/s/2v86piOgtK_t--Pzu28LgQ)
- [Generating Adversarial Malware Examples for Black-Box Attacks Based on GAN](https://arxiv.org/abs/1702.05983)

## 攻击AI ##
### 攻击AI基础框架 ###
- [深度学习框架中的魔鬼——探究人工智能系统中的安全问题](https://www.anquanke.com/post/id/86989)
- [对深度学习的降维攻击 — 人工智能系统数据流中的安全风险](https://www.anquanke.com/post/id/95095)
- [DEFCON CHINA议题解读 | 对深度学习系统的数据流攻击](https://www.anquanke.com/post/id/144837)
- [AI繁荣下的隐忧——Google Tensorflow安全风险剖析](https://security.tencent.com/index.php/blog/msg/130)

### 攻击AI数据/模型/系统 ###
- [安全领域中机器学习的对抗和博弈](http://bindog.github.io/blog/2016/11/13/game-playing-with-ml-in-security/)
- [基础攻防场景下的AI对抗样本初探](https://www.cdxy.me/?p=798)
- [使用生成对抗网络(GAN)生成DGA](http://webber.tech/posts/%E4%BD%BF%E7%94%A8%E7%94%9F%E6%88%90%E5%AF%B9%E6%8A%97%E7%BD%91%E7%BB%9C%28GAN%29%E7%94%9F%E6%88%90DGA/)
- [详解如何使用Keras实现Wassertein GAN](https://mp.weixin.qq.com/s/F2gBP23LCEF72QDlugbBZQ)
- [Is attacking machine learning easier than defending it?](http://www.cleverhans.io/security/privacy/ml/2017/02/15/why-attacking-machine-learning-is-easier-than-defending-it.html)
- [对深度学习的逃逸攻击 ——探究人工智能系统中的安全盲区](https://www.anquanke.com/post/id/87037)
- [NLP机器学习模型安全性及实践](https://bbs.pediy.com/thread-230125.htm)
- [机器学习对抗性攻击报告](https://mp.weixin.qq.com/s/QKXd9AKkVwk3CO45-BbZSA?)
- [从安全视角对机器学习的部分思考](https://mp.weixin.qq.com/s/kP4YuiksI1dfZdT8Z_j_cQ)
- [污染TensorFlow模型: XCTF 2019 Final tfboys命题思路](https://www.cdxy.me/?p=813)
- [中科院信工所发布《深度学习系统的隐私与安全》综述论文，187篇文献总结](https://mp.weixin.qq.com/s/B0FTTAppy_AUt6SXVFL-Pg)
- [Towards Privacy and Security of Deep Learning Systems: A Survey](https://arxiv.org/pdf/1911.12562v1.pdf)

# 心得体会篇
1. 随着学习门槛的提高，公开的工业界资料已经相对匮乏，所以开始学习一些学术界较新的paper，理解吃透再工程化。
2. Reinforcement Learning + Deep Learning = AI
3. 人工智能技术应用于网络安全等各个垂直领域已经是大势所趋（虽然不得不承认有其局限性，但是我们可以通过细划分场景有针对性的进行安全问题分解、抽象，结合机器学习技术解决问题）
4. 对安全场景、攻击模式、数据的认识深度，远比选择工具重要
5. 加高自己的技术壁垒：业务业务业务，锻炼业务敏感性，理解业务需求，给出解决方案（基于业务的特征工程）
6. 万物皆规则，机器学习训练的模型也是一种规则。用传统规则还是机器学习模型规则取决于对业务场景的先验知识的掌握程度。

# 学习交流篇
为适配（碎片化时间）移动端阅读与知识传播，后续持续更新内容，将同步在个人微信公众号：404 Not F0und，同时公众号提供了该项目的PDF版本，关注后回复"智能安全" 即可下载。公众号致力于分享原创高质量干货，包括但不限于：应用安全、机器智能、安全算法、安全数据分析、企业安全建设。知识分享的价值在于既能系统化梳理自己的研究和思考，又可能和他人思维碰撞，发生一些有意思的事情。​

![](https://i.imgur.com/C9qsWz6.jpg)






