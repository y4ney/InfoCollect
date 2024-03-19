# 信息收集

## 1 域名信息

### 1.1 whois查询

> 🚥 简单来说Whois就是一个用于查询域名是否已被注册以及注册域名的详细信息的数据库，可用于收集网络注册信息，注册的域名，IP地址等信息。
>
> 注册人的姓名和邮箱信息通常对测试个人站点非常有用，因为我们可以通过搜索引擎和社交网络挖掘处域名所有人的很多信息。对于中小站点而言，域名所有人往往就是管理员。
>
> 需要注意的信息有：域名服务商、域名拥有者、以及他们的邮箱、电话、地址。

- whois 命令
- 爱站网：[https://whois.aizhan.com/](https://whois.aizhan.com/ "https://whois.aizhan.com/")
- 站长之家：[https://whois.chinaz.com/](https://whois.chinaz.com/ "https://whois.chinaz.com/")

### 1.2 备案信息查询

> 🚥  网站备案是根据国家法律法规规定，需要网站的所有者向国家有关部门申请的备案，这是国家信息产业部对网站的一种管理，为了防止在网上从事非法的网站经营活动的发生。
>
> 主要针对国内网站，如果网站搭建在其他国家，则不需要进行备案。

- 天眼查：[https://www.tianyancha.com/](https://www.tianyancha.com/ "https://www.tianyancha.com/")
- 站长工具：[https://icp.chinaz.com/](https://icp.chinaz.com/ "https://icp.chinaz.com/")
- ICP备案查询网：[https://www.beianx.cn/](https://www.beianx.cn/ "https://www.beianx.cn/")
- 查IP：[https://www.chaicp.com/](https://www.chaicp.com/ "https://www.chaicp.com/")

### 1.3 子域名收集

- OneForAll：[https://github.com/shmilylty/OneForAll](https://github.com/shmilylty/OneForAll "https://github.com/shmilylty/OneForAll")
- Sublist3r：[https://github.com/aboul3la/Sublist3r](https://github.com/aboul3la/Sublist3r "https://github.com/aboul3la/Sublist3r")
- K8：[https://github.com/k8gege/K8tools](https://github.com/k8gege/K8tools "https://github.com/k8gege/K8tools")
- Layer子域名挖掘机：[https://github.com/euphrat1ca/LayerDomainFinder](https://github.com/euphrat1ca/LayerDomainFinder "https://github.com/euphrat1ca/LayerDomainFinder")
- wydomain：[https://github.com/ring04h/wydomain](https://github.com/ring04h/wydomain "https://github.com/ring04h/wydomain")
- Sublist3r：[https://github.com/aboul3la/Sublist3r](https://github.com/aboul3la/Sublist3r "https://github.com/aboul3la/Sublist3r")
    > 🚥 Sublist3r能列举多种资源，如在Google、Yahoo、Bing、Baidu和Ask等搜索引擎中可查到的子域名，还可以列出Netcraft、VirusTotal、ThreatCrowd、DNSdumpster和Reverse DNS查到的子域名。
- dnsmaper：[https://github.com/le4f/dnsmaper](https://github.com/le4f/dnsmaper "https://github.com/le4f/dnsmaper")
- subDomainsBrute：[https://github.com/lijiejie/subDomainsBrute](https://github.com/lijiejie/subDomainsBrute "https://github.com/lijiejie/subDomainsBrute")
- Maltego CE：[https://www.maltego.com/](https://www.maltego.com/ "https://www.maltego.com/")
- Subfinder：[https://github.com/projectdiscovery/subfinder](https://github.com/projectdiscovery/subfinder "https://github.com/projectdiscovery/subfinder")
    > 🚥 一个汇集了 7 种 API 的子域发现工具，可通过使用被动的在线资源来发现网站的有效子域。它具有简单的模块化架构，并针对速度进行了优化。
- DNSdumpster：[https://dnsdumpster.com/](https://dnsdumpster.com/ "https://dnsdumpster.com/")
    > 🚥 很多第三方服务汇聚了大量DNS数据集，可通过它们检索某个给定域名的子域名。读者也可以利用DNSdumpster网站、在线DNS侦查和搜索的工具挖掘出指定域潜藏的大量子域。
- IP反查绑定域名网站：[https://dns.aizhan.com/](https://dns.aizhan.com/ "https://dns.aizhan.com/")
- 证书透明度查询
    > 🚥  证书透明度（Certificate Transparency，CT）是证书授权机构（CA）的一个项目，证书授权机构会将每个SSL/TLS证书发布到公共日志中。一个SSL/TLS证书通常包含域名、子域名和邮件地址，这些也经常成为攻击者非常希望获得的有用信息。查找某个域名所属证书的最简单的方法就是使用搜索引擎搜索一些公开的CT日志。

  - crt.sh：[https://crt.sh/](https://crt.sh/ "https://crt.sh/")

  - censys.io：[https://censys.com/](https://censys.com/ "https://censys.com/")
- esd：[https://github.com/FeeiCN/ESD](https://github.com/FeeiCN/ESD "https://github.com/FeeiCN/ESD")
    > 🚥 优势：
    >
    > 1. 支持泛解析域名
    > 2. 基于RSC（响应相似度对比）技术对泛解析域名进行枚举（受网络质量、网站带宽等影响，速度会比较慢）
    > 3. 基于aioHTTP获取一个不存在子域名的响应内容，并将其和字典子域名响应进行相似度比对。 超过阈值则说明是同个页面，否则则为可用子域名，并对最终子域名再次进行响应相似度对比。
    >     更快的速度
    > 4. 基于AsyncIO异步协程技术对域名进行枚举（受网络和DNS服务器影响会导致扫描速度小幅波动，基本在250秒以内）
    > 5. 基于AsyncIO+aioDNS将比传统多进程/多线程/gevent模式快50%以上。 通过扫描qq.com，共170083条规则，找到1913个域名，耗时163秒左右，平均1000+条/秒。
    > 6. 更全的字典
    > 7. 融合各类字典，去重后共170083条子域名字典

### 2 IP 信息

> 🚥 CDN即内容分发网络，主要解决因传输距离和不同运营商节点造成的网络速度性能低下的问题。说得简单点，就是一组在不同运营商之间的对接节点上的高速缓存服务器，把用户经常访问的静态数据资源（例如静态的html、css、js图片等文件）直接缓存到节点服务器上，当用户再次请求时，会直接分发到在离用户近的节点服务器上响应给用户，当用户有实际数据交互时才会从远程Web服务器上响应，这样可以大大提高网站的响应速度及用户体验。

### 2.1 是否存在CDN

> 🚥 通常会通过ping目标主域，观察域名的解析情况，以此来判断其是否使用了CDN

- 17CE：[https://www.17ce.com/](https://www.17ce.com/ "https://www.17ce.com/")
    > 🚥 利用在线网站17CE进行全国多地区的ping服务器操作，然后对比每个地区ping出的IP结果，查看这些IP是否一致，如果都是一样的，极有可能不存在CDN。如果IP大多不太一样或者规律性很强，可以尝试查询这些IP的归属地，判断是否存在CDN。

### 2.2 不存在CDN

- IP查询：[https://www.ip138.com/](https://www.ip138.com/ "https://www.ip138.com/")

### 2.3 绕过CDN，如何绕过

- 内部邮箱源
    > 🚥 一般的邮件系统都在内部，没有经过CDN的解析，通过目标网站用户注册或者RSS订阅功能，查看邮件、寻找邮件头中的邮件服务器域名IP，ping这个邮件服务器的域名，就可以获得目标的真实IP
    >
    > 注意，必须是目标自己的邮件服务器，第三方或公共邮件服务器是没有用的。
- 扫描网站测试文件
    > 🚥 如phpinfo、test等，从而找到目标的真实IP。
- 分站域名
    > 🚥 很多网站主站的访问量会比较大，所以主站都是挂CDN的，但是分站可能没有挂CDN，可以通过ping二级域名获取分站IP，可能会出现分站和主站不是同一个IP但在同一个C段下面的情况，从而能判断出目标的真实IP段。
- 国外访问
    > 🚥  国内的CDN往往只对国内用户的访问加速，而国外的CDN就不一定了。因此，通过国外在线代理网站访问，可能会得到真实的IP

  - [AppSynthetic Monitor](https://api.asm.saas.broadcom.com//v3/oauth2/auth?client_id=1\&response_type=code\&state=1642669822\&redirect_uri=https%3A%2F%2Fasm.saas.broadcom.com%2F%2Fen%2Fcore%2Fauth%2FaccessToken\&lang=en "AppSynthetic Monitor")
- 查询域名的解析记录

    > 🚥  也许目标很久以前并没有用过CDN，所以可以通过网站NETCRAFT来观察域名的IP历史记录，也可以大致分析出目标的真实IP段。

  - NETCRAFT：[https://www.netcraft.com/](https://www.netcraft.com/ "https://www.netcraft.com/")
- App的请求
    > 🚥  如果目标网站有自己的App，可以尝试利用Fiddler或BurpSuite抓取App的请求，从里面找到目标的真实IP。

### 2.4 验证获取的IP

> 🚥  直接尝试用IP访问，看看响应的页面是不是和访问域名返回的一样；或者在目标段比较大的情况下，借助类似Masscan的工具批扫描对应IP段中所有开了80、443、8080端口的IP，然后逐个尝试IP访问，观察响应结果是否为目标站点。

## 3 端口信息

> 🚥  在渗透测试的过程中，对端口信息的收集是一个很重要的过程，通过扫描服务器开放的端口以及从该端口判断服务器上存在的服务，就可以对症下药，便于我们渗透目标服务器。我们需要关注常见应用的默认端口和在端口上运行的服务。

- Nmap：[https://github.com/nmap/nmap](https://github.com/nmap/nmap "https://github.com/nmap/nmap")
    > 🚦推荐使用命令
    >
    > ```bash
    > nmap -T4 -A -v -Pn xxx.com
    > ```

- masscan：[https://github.com/robertdavidgraham/masscan](https://github.com/robertdavidgraham/masscan "https://github.com/robertdavidgraham/masscan")
- ZMap：[https://github.com/zmap/zmap](https://github.com/zmap/zmap "https://github.com/zmap/zmap")
- 御剑TCP端口扫描工具：[https://github.com/foryujian/yjdirscan](https://github.com/foryujian/yjdirscan "https://github.com/foryujian/yjdirscan")
- Gorailgun：[https://github.com/lz520520/railgun](https://github.com/lz520520/railgun "https://github.com/lz520520/railgun")
- 站长之家：[https://tool.chinaz.com/port](https://tool.chinaz.com/port "https://tool.chinaz.com/port")
- PostJson：[http://coolaf.com/tool/port](http://coolaf.com/tool/port "http://coolaf.com/tool/port")

| 端口号      | 端口说明           | 攻击方向               |
| -------- | -------------- | ------------------ |
| 21/22/69 | FTP/TFTP文件传输协议 | 允许匿名的上传、下载、爆破和嗅探操作 |
| 2049     | NFS服务          | 配置不当               |
| 139      | samba服务        | 爆破、未授权访问、远程代码执行    |
| 389      | LDAP目录访问协议     | 注入、允许匿名访问、弱口令      |

| 端口号  | 端口说明         | 攻击方向                                   |
| ---- | ------------ | -------------------------------------- |
| 22   | SSH远程连接      | 爆破、SSH隧道以及内网代理转发、文件传输                  |
| 23   | Telnet远程连接   | 爆破、嗅探、弱口令                              |
| 3389 | RDP远程桌面连接    | Shift后门（需要Windows Server 2003以下的系统）、爆破 |
| 5900 | VNC          | 弱口令爆破                                  |
| 5632 | PyAnywhere服务 | 抓密码、代码执行                               |

| 端口号         | 端口说明                      | 攻击方向               |
| ----------- | ------------------------- | ------------------ |
| 80/443/8080 | 常见的Web服务端口                | Web攻击、爆破、对应服务器版本漏洞 |
| 7001/7002   | WebLogic控制台               | Java反序列化、弱口令       |
| 8080/8089   | Jboss/Resin/Jetty/Jenkins | 反序列化、控制台弱口令        |
| 9090        | WebSphere控制台              | Java反序列化、弱口令       |
| 4848        | GlassFish控制台              | 弱口令                |
| 1352        | Lotus domino邮件服务          | 弱口令、信息泄漏、爆破        |
| 10000       | Webmin-Web控制面板            | 弱口令                |

| 端口号         | 端口说明           | 攻击方向             |
| ----------- | -------------- | ---------------- |
| 3306        | MySQL          | 注入、提权、爆破         |
| 1433        | MSSQL数据库       | 注入、提权、SA弱口令、爆破   |
| 1521        | Oracle数据库      | TNS爆破、注入、反弹Shell |
| 5432        | PostgreSQL数据库  | 爆破、注入、弱口令        |
| 27017/27018 | MongoDB        | 爆破、未授权访问         |
| 6379        | Redis数据库       | 可尝试未授权访问、弱口令爆破   |
| 5000        | SysBase/DB2数据库 | 爆破、注入            |

| 端口号 | 端口说明     | 攻击方向  |
| --- | -------- | ----- |
| 25  | SMTP邮件服务 | 邮件伪造  |
| 110 | POP3协议   | 爆破、嗅探 |
| 143 | IMAP协议   | 爆破    |

| 端口号   | 端口说明    | 攻击方向                 |
| ----- | ------- | -------------------- |
| 53    | DNS域名服务 | 允许区域传送、DNS劫持、缓存偷渡、欺骗 |
| 67/68 | DHCP服务  | 劫持、欺骗                |
| 161   | SNMP服务  | 爆破、搜集目标内网信息          |

| 端口号         | 端口说明                  | 攻击方向        |
| ----------- | --------------------- | ----------- |
| 2181        | Zookeeper服务           | 未授权访问       |
| 8069        | Zabbix服务              | 远程执行、SQL注入  |
| 9200/9300   | Elasticsearch服务       | 远程执行        |
| 11211       | Memcache服务            | 未授权访问       |
| 512/513/514 | Linux Rexec服务         | 爆破、Rlogin登陆 |
| 873         | Rsync服务               | 匿名访问、文件上传   |
| 3690        | Svn服务                 | Svn泄漏、未授权访问 |
| 50000       | SAP Management Consle | 远程执行        |

## 4 指纹信息

- F12查看数据包响应头
- wappalyzer：[https://chromewebstore.google.com/detail/wappalyzer-technology-pro/gppongmhjkpfnbhagpmjfkannfbllamg](https://chromewebstore.google.com/detail/wappalyzer-technology-pro/gppongmhjkpfnbhagpmjfkannfbllamg "https://chromewebstore.google.com/detail/wappalyzer-technology-pro/gppongmhjkpfnbhagpmjfkannfbllamg")
- WhatWeb：[https://github.com/urbanadventurer/WhatWeb](https://github.com/urbanadventurer/WhatWeb "https://github.com/urbanadventurer/WhatWeb")
- CMSeeK：[https://github.com/Tuhinshubhra/CMSeeK](https://github.com/Tuhinshubhra/CMSeeK "https://github.com/Tuhinshubhra/CMSeeK")
- CMSmap：[https://github.com/Dionach/CMSmap](https://github.com/Dionach/CMSmap "https://github.com/Dionach/CMSmap")
- ACMSDiscovery：[https://github.com/aedoo/ACMSDiscovery](https://github.com/aedoo/ACMSDiscovery "https://github.com/aedoo/ACMSDiscovery")
- TideFinger：[https://github.com/TideSec/TideFinger](https://github.com/TideSec/TideFinger "https://github.com/TideSec/TideFinger")
- AngelSword：[https://github.com/Lucifer1993/AngelSword](https://github.com/Lucifer1993/AngelSword "https://github.com/Lucifer1993/AngelSword")
- 御剑Web指纹识别：[https://www.xitongzhijia.net/soft/171203.html](https://www.xitongzhijia.net/soft/171203.html "https://www.xitongzhijia.net/soft/171203.html")
- 云悉指纹：[https://www.yunsee.cn/](https://www.yunsee.cn/ "https://www.yunsee.cn/")
- WhatWeb在线版：[https://whatweb.net/](https://whatweb.net/ "https://whatweb.net/")
- 潮汐指纹：[http://finger.tidesec.com/](http://finger.tidesec.com/ "http://finger.tidesec.com/")

## 5 敏感信息

- 搜索引擎
    > 🚥  可以利用搜索引擎收集数据库文件、SQL注入、配置信息、源代码泄漏、未授权访问和robots.txt等敏感信息。
  - Google：[https://www.google.com.hk/](https://www.google.com.hk/ "https://www.google.com.hk/")
  - baidu：[https://www.baidu.com/](https://www.baidu.com/ "https://www.baidu.com/")
  - 雅虎：[https://www.yahoo.com/](https://www.yahoo.com/ "https://www.yahoo.com/")
  - Bing：[https://www.bing.com/](https://www.bing.com/ "https://www.bing.com/")
  - shodan：[https://chrome.google.com/webstore/detail/jjalcfnidlmpjhdfepjhjbhnhkbgleap](https://chrome.google.com/webstore/detail/jjalcfnidlmpjhdfepjhjbhnhkbgleap "https://chrome.google.com/webstore/detail/jjalcfnidlmpjhdfepjhjbhnhkbgleap")

    | 关键字      | 说明                                                                        |
    | -------- | ------------------------------------------------------------------------- |
    | site     | 指定域名。搜索学校网站的后台：`site:edu.cn intext:后台管理`（搜索网页正文中含有“后台管理”并且域名后缀是edu.cn的网站） |
    | inurl    | URL中存在关键字的网页                                                              |
    | intext   | 网页正文中的关键字                                                                 |
    | filetype | 制定文件类型                                                                    |
    | intitle  | 网页标题中的关键字                                                                 |
    | link     | `link:baidu.com`即表示返回所有和baidu.com做了链接的URL                                 |
    | info     | 查找指定站点的一些基本信息                                                             |
    | cache    | 搜索google里关于某些内容的缓存                                                        |

- Burp Suite：
    > 🚥  通过Repeater功能同样可以获取一些服务器的信息。
  - Server头和X-Powered-By头会暴露目标服务器和使用的编程语言信息。
  - 抓取经过的数据报文，搜索关键字。
- github
    > 🚥  可以在Github上搜索数据库连接信息、邮箱密码、uc-key、阿里的osskey、源代码泄漏。
  - gsil：[https://github.com/FeeiCN/GSIL](https://github.com/FeeiCN/GSIL "https://github.com/FeeiCN/GSIL")
  - gshark：[https://github.com/madneal/gshark](https://github.com/madneal/gshark "https://github.com/madneal/gshark")
    | 邮件配置信息泄露 | site:Github.com smtp、site:Github.com <smtp@qq.com>                                               |
    | -------- | ----------------------------------------------------------------------------------------------- |
    | 数据库信息泄露  | site:Github.com sa password、site:Github.com root password、site:Github.com User ID=‘sa’;Password |
    | svn信息泄露  | site:Github.com svn、site:Github.com svn username                                                |
    | 综合信息泄露   | site:Github.com password、site:Github…com ftp ftppassword                                        |
- 乌云漏洞表：[http://wooyun.2xss.cc/](http://wooyun.2xss.cc/ "http://wooyun.2xss.cc/")
    > 🚥  通过乌云漏洞表查询历史漏洞信息
- CSDN：[https://so.csdn.net/so/search?](https://so.csdn.net/so/search? "https://so.csdn.net/so/search?")
- 语雀：[语雀公开信息搜索引擎](https://www.yuque.com/search?q=\&type=content\&scope=%2F\&tab=public\&p=1\&sence=searchPage "语雀公开信息搜索引擎")
    > 🚥  语雀是一个企业级协作服务，提供文档、表格、项目管理等协作工具，帮助企业沉淀、整理内部信息和知识。很多团队都会使用语雀来搭建知识库，所以难免有些人员安全意识不足，将敏感信息放到了语雀在线公开文档中，从而导致信息泄漏。
    >
    > 我们可以通过语雀的引擎搜索企业的关键字，例如：域名、企业简称、软件名称、账号、密码和企业的特别称呼等等。
- 社交媒体用户信息
    > 🚥  Sherlock Project提供了一个非常强大的命令行工具Sherlock来查找社交网络（社交网络列表及规则可自定义扩展延伸）中的用户名。
  - Sherlock：[https://github.com/sherlock-project/sherlock](https://github.com/sherlock-project/sherlock "https://github.com/sherlock-project/sherlock")
- 简书：[https://www.jianshu.com/search?](https://www.jianshu.com/search? "https://www.jianshu.com/search?")
- DumpsterDiver ：[https://github.com/securing/DumpsterDiver](https://github.com/securing/DumpsterDiver "https://github.com/securing/DumpsterDiver")
    > 🚥  可以分析大量数据以搜索硬编码的密钥或密码。此外，它还允许创建具有基本条件的简单搜索规则。
- JS信息
  - JSFinder：[https://github.com/Threezh1/JSFinder](https://github.com/Threezh1/JSFinder "https://github.com/Threezh1/JSFinder")
  - FindSomething：[https://github.com/momosecurity/FindSomething](https://github.com/momosecurity/FindSomething "https://github.com/momosecurity/FindSomething")
  - subjs：[https://github.com/lc/subjs](https://github.com/lc/subjs "https://github.com/lc/subjs")
  - linkfinder：[https://github.com/GerbenJavado/LinkFinder](https://github.com/GerbenJavado/LinkFinder "https://github.com/GerbenJavado/LinkFinder")
  - subfinder：[https://github.com/projectdiscovery/subfinder](https://github.com/projectdiscovery/subfinder "https://github.com/projectdiscovery/subfinder")
  - httpx [https://github.com/projectdiscovery/httpx](https://github.com/projectdiscovery/httpx "https://github.com/projectdiscovery/httpx")
  - gau [https://github.com/lc/gau](https://github.com/lc/gau "https://github.com/lc/gau")
  - waybackurls [https://github.com/tomnomnom/waybackurls](https://github.com/tomnomnom/waybackurls "https://github.com/tomnomnom/waybackurls")
  - hakrawler [https://github.com/hakluke/hakrawler](https://github.com/hakluke/hakrawler "https://github.com/hakluke/hakrawler")
  - 利用爬虫获取全站链接：[https://commoncrawl.org/](https://commoncrawl.org/ "https://commoncrawl.org/")
  - 搜索网页存档中的JS信息：[http://archive.org/](http://archive.org/ "http://archive.org/")

    > 🚥  国内有时候不稳定，多刷新
  
  - nipejs：[https://github.com/i5nipe/nipejs](https://github.com/i5nipe/nipejs "https://github.com/i5nipe/nipejs")
  - katana：[https://github.com/projectdiscovery/katana](https://github.com/projectdiscovery/katana "https://github.com/projectdiscovery/katana")

      > 🚦爬取xxx.com网站下的所有js文件，并获取其中的敏感数据：
      >
      > ```bash
      > echo xxx.com | katana | grep ".\bjs\b" | nipejs -r ~/.config/nipejs/regex.txt
      > ```
      >
- 网盘信息
- App信息
  - AppInfoScanner：[https://github.com/kelvinBen/AppInfoScanner](https://github.com/kelvinBen/AppInfoScanner "https://github.com/kelvinBen/AppInfoScanner")
  - APKLeaks：[https://github.com/dwisiswant0/apkleaks](https://github.com/dwisiswant0/apkleaks "https://github.com/dwisiswant0/apkleaks")
  - 检查客户端程序存储在手机中的 SharedPreferences 配置文件
  - 检查客户端程序存储在手机中的 SQLite 数据库文件
  - 检查客户端程序 apk 包中是否保存有敏感信息（反编译、逆向、检查apk包中各类文件是否包含硬编码的敏感信息）
  - logcat日志

## 6 目录信息

- dirsearch：[https://github.com/maurosoria/dirsearch](https://github.com/maurosoria/dirsearch "https://github.com/maurosoria/dirsearch")
- DirBuster：[https://github.com/KajanM/DirBuster](https://github.com/KajanM/DirBuster "https://github.com/KajanM/DirBuster")
    > 🚥  DirBuster是OWASP开发的一款基于Java编写的、专门用于探测Web服务器的目录和隐藏文件。
- 御剑后台扫描珍藏版：[https://pan.baidu.com/share/init?surl=MJN\_ldSFZAk72pe4DkffHA](https://pan.baidu.com/share/init?surl=MJN_ldSFZAk72pe4DkffHA "https://pan.baidu.com/share/init?surl=MJN_ldSFZAk72pe4DkffHA")
  - 提取码: y9wj
  - 解压密码：www.fujieace.com
- wwwscan：[https://github.com/aducode/wwwscan](https://github.com/aducode/wwwscan "https://github.com/aducode/wwwscan")
- Sensitivefilescan：[https://github.com/aipengjie/sensitivefilescan](https://github.com/aipengjie/sensitivefilescan "https://github.com/aipengjie/sensitivefilescan")
    > 🚥  轻量级快速单文件目录后台扫描
- Weakfilescan：[https://github.com/ring04h/weakfilescan](https://github.com/ring04h/weakfilescan "https://github.com/ring04h/weakfilescan")
    > 🚥  轻量级快速单文件目录后台扫描
- WebScan：[https://www.webscan.cc/](https://www.webscan.cc/ "https://www.webscan.cc/")
- Gospider：[https://github.com/jaeles-project/gospider](https://github.com/jaeles-project/gospider "https://github.com/jaeles-project/gospider")
- Cansina：[https://github.com/deibit/cansina](https://github.com/deibit/cansina "https://github.com/deibit/cansina")
- YuhScan：[https://github.com/0xhunya/yuhScan](https://github.com/0xhunya/yuhScan "https://github.com/0xhunya/yuhScan")

## 7 网络空间测绘

- FOFA：[https://fofa.info/](https://fofa.info/ "https://fofa.info/")
    > 🚥  支持很多语法结果组合查询（domain、title、ip、header、body），能够更快的获取目标站点的信息
- Hunter：[https://hunter.qianxin.com/](https://hunter.qianxin.com/ "https://hunter.qianxin.com/")
    > 🚥 这款工具是奇安信全球鹰实验室研发的一款空间测绘工具，每天有免费次数，有钱的大哥可以奢侈一把。
- Zoomeye：[https://www.zoomeye.org/](https://www.zoomeye.org/ "https://www.zoomeye.org/")
- quake：[https://quake.360.cn/quake/#/index](https://quake.360.cn/quake/#/index "https://quake.360.cn/quake/#/index")
- shodan：[https://www.shodan.io/](https://www.shodan.io/ "https://www.shodan.io/")

## 8 病毒扫描

- Virustotal：[https://www.virustotal.com/gui/](https://www.virustotal.com/gui/ "https://www.virustotal.com/gui/")

## 9 参考案例

- [Sherlock：在社交网络中查找用户名的信息收集工具](https://mp.weixin.qq.com/s?__biz=MzUyMTA0MjQ4NA==\&mid=2247548805\&idx=2\&sn=fff911f5fead7684d1e63f25a1c9c18f "Sherlock：在社交网络中查找用户名的信息收集工具")
- [渗透测试---信息收集(细!)](https://xz.aliyun.com/t/9994?time__1311=n4%2BxuDgD9AeWqBKD%3DKDsD7feYg40xiKeNe5PN4x\&alichlgref=https%3A%2F%2Fwww.google.com.hk%2F "渗透测试---信息收集(细!)")
- [多种文件类型中敏感信息搜索工具](https://www.wevul.com/2713.html "多种文件类型中敏感信息搜索工具")
- [推荐两款github敏感信息搜集工具（gsil、gshark）](https://cloud.tencent.com/developer/article/1757828 "推荐两款github敏感信息搜集工具（gsil、gshark）")
- [信息收集系列之JavaScript文件敏感信息提取](https://zone.huoxian.cn/d/336-javascript "信息收集系列之JavaScript文件敏感信息提取")
- [观模丨浅谈Web渗透之信息收集（下）](https://51fusa.com/client/knowledge/knowledgedetail/id/3494.html "观模丨浅谈Web渗透之信息收集（下）")
- [一、信息收集-4.敏感信息收集](https://blog.csdn.net/Mr_lingyuhong/article/details/134162904 "一、信息收集-4.敏感信息收集")
- [APP敏感信息收集技巧](https://forum.butian.net/question/1030 "APP敏感信息收集技巧")
- [YY运维不当导致(可内网/jumserver/新机房交换机帐号密码等/其他重要敏感信息泄露)](http://www.wooyun.org/bugs/wooyun-2016-0206981 "YY运维不当导致(可内网/jumserver/新机房交换机帐号密码等/其他重要敏感信息泄露)")
- [京东商城某员工邮箱到1091名员工企业邮箱账号泄露(存在撞库和社工风险)](http://www.wooyun.org/bugs/wooyun-2016-0194367 "京东商城某员工邮箱到1091名员工企业邮箱账号泄露(存在撞库和社工风险)")
- [bilibili安卓客户端源码泄露（2016年1月的版本）](http://www.wooyun.org/bugs/wooyun-2016-0193492 "bilibili安卓客户端源码泄露（2016年1月的版本）")
- [自如网某漏洞涉及各种敏感信息(数据库配置/邮箱/mongoDB等)](http://www.wooyun.org/bugs/wooyun-2010-0193492 "自如网某漏洞涉及各种敏感信息(数据库配置/邮箱/mongoDB等)")
- [百度移动游戏内部邮箱账号泄露](http://www.wooyun.org/bugs/wooyun-2015-0157841 "百度移动游戏内部邮箱账号泄露")
- [阿里巴巴少量内部敏感信息泄漏](http://www.wooyun.org/bugs/wooyun-2015-093240 "阿里巴巴少量内部敏感信息泄漏")
- [信息收集技巧 | 从JS中获得敏感信息](https://cn-sec.com/archives/1797889.html "信息收集技巧 | 从JS中获得敏感信息")
- [挖洞Bounty Tips | js中的敏感信息收集](https://cn-sec.com/archives/965728.html "挖洞Bounty Tips | js中的敏感信息收集")
- [APKLeaks：APK敏感信息收集工具](https://www.wevul.com/1742.html "APKLeaks：APK敏感信息收集工具")
