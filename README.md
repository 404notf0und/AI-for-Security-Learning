# AI-for-Security-Learning
安全场景、基于AI的安全算法和安全数据分析学习笔记

项目地址：https://github.com/404notf0und/AI-for-Security-Learning

最近更新日期为：2018/11/22

同步更新于：404 Not Found：AI for Security

目录：
- [AI for Security Learning](#AI-for-Security-Learning)
	- [防护篇](#防护篇)
		- [恶意软件&代码](#恶意软件&代码)
		- [恶意流量检测](#恶意流量检测)
		- [域名安全](#域名安全)
		- [业务安全](#业务安全)
		- [Web安全](#Web安全)
			- [URL异常检测](#URL异常检测)
			- [XSS检测](#XSS检测)
			- [Web攻击多分类检测](#Web攻击多分类检测)
			- [Webshell检测](#Webshell检测)
		- [其他安全检测](#其他安全检测)
			- [WindowsRDP检测]
			- [PowerShell检测]
			- [用户行为(UBA)检测]
			- [弱口令检测]
	- [对抗篇](#对抗篇)
		- [对抗样本](#对抗样本)

<!-- more -->

# AI for Security Learning
## 防护篇 ##
### 恶意软件&代码 ###
- [深度学习在恶意软件检测中的应用](https://xz.aliyun.com/t/2447)
- [恶意软件与数据分析](https://iami.xyz/AliSEC3/)
- [利用机器学习进行恶意代码分类](http://drops.xmd5.com/static/drops/tips-8151.html)
- [用机器学习检测Android恶意代码](http://drops.xmd5.com/static/drops/mobile-13428.html)
- [Malware Detection in Executables Using Neural Networks](https://devblogs.nvidia.com/malware-detection-neural-networks/)

### 恶意流量检测 ###
**- [利用机器学习检测HTTP恶意外连流量](https://www.freebuf.com/column/170483.html)**

### 域名安全 ###
- [机器学习与威胁情报的融合：一种基于AI检测恶意域名的方法](https://www.freebuf.com/articles/es/187451.html)
- [使用fasttext进行DGA检测](https://iami.xyz/DGA-Detect/)
- [使用CNN检测DNS隧道](https://github.com/BoneLee/dns_tunnel_dectect_with_CNN)

### 业务安全 ###
- [基于设备指纹的风控建模以及机器学习的尝试](https://xz.aliyun.com/t/2801)
- [如何在安全风控中评估和量化机器学习有效性](https://xz.aliyun.com/t/2951)

### Web安全 ###
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

### 其他安全检测 ###
- [机器学习在WindowsRDP版本和后门检测上的应用](https://www.anquanke.com/post/id/157175)
- [用机器学习检测恶意PowerShell](https://xz.aliyun.com/t/2437)
- [机器学习算法在用户行为检测(UBA)领域的应用](http://dearcharles.cn/2017/11/11/%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%E7%AE%97%E6%B3%95%E5%9C%A8%E7%94%A8%E6%88%B7%E8%A1%8C%E4%B8%BA%E6%A3%80%E6%B5%8B-UBA-%E9%A2%86%E5%9F%9F%E7%9A%84%E5%BA%94%E7%94%A8/)
- [利用机器学习和规则实现弱口令检测](https://manning23.github.io/2018/10/12/%E5%88%A9%E7%94%A8%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%E5%92%8C%E8%A7%84%E5%88%99%E5%AE%9E%E7%8E%B0%E5%BC%B1%E5%8F%A3%E4%BB%A4%E6%A3%80%E6%B5%8B/)

## 对抗篇 ##
### 对抗样本 ###
- [安全领域中机器学习的对抗和博弈](http://bindog.github.io/blog/2016/11/13/game-playing-with-ml-in-security/)
- [基础攻防场景下的AI对抗样本初探](https://www.cdxy.me/?p=798)
- [AI与安全的恩怨情仇五部曲「1」Misuse AI](https://www.zuozuovera.com/archives/1565/)
- [机器学习在安全攻防场景的应用与分析](https://www.freebuf.com/articles/neopoints/152457.html)
- [使用生成对抗网络(GAN)生成DGA](http://webber.tech/posts/%E4%BD%BF%E7%94%A8%E7%94%9F%E6%88%90%E5%AF%B9%E6%8A%97%E7%BD%91%E7%BB%9C%28GAN%29%E7%94%9F%E6%88%90DGA/)
- [详解如何使用Keras实现Wassertein GAN](https://mp.weixin.qq.com/s/F2gBP23LCEF72QDlugbBZQ)
- [Is attacking machine learning easier than defending it?](http://www.cleverhans.io/security/privacy/ml/2017/02/15/why-attacking-machine-learning-is-easier-than-defending-it.html)
