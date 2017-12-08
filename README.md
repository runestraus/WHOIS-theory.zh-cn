WHOIS theory
=========================
WHOIS 理论资料整理,中文

## WHOIS 简介&历史
> WHOIS (pronounced as the phrase who is) is a query and response protocol      
> that is widely used for querying databases that store the registered users or assignees of an Internet resource,      
> such as a domain name, an IP address block, or an autonomous system, 
> but is also used for a wider range of other information. 
> The protocol stores and delivers database content in a human-readable format.

WHOIS（读作“Who is”，而非缩写）是用来查询互联网中域名的IP以及所有者等信息的传输协议。      
主要被被使用于查询域名和IP的注册相关信息.      

### 简史
当互联网脱离ARPANET时，只有一个组织处理所有域名注册，即DARPA本身。在RFC 920中建立了注册流程.        
20世纪80年代初，WHOIS被标准化，用于查找与域名和号码(IP)的注册相关的域，人员和其他资源。      
**由于当时所有的注册都是由一个组织完成的，所以一个中央服务器用于WHOIS查询。这使得查找这样的信息非常容易。**      

在20世纪80年代ARPANET成为互联网的时候，域名的注册仍然是DARPA的责任与工作。       
随后UUNET开始提供域名注册服务,但他们只是处理这些注册信息文件转交给DARPA网络信息中心（NIC）的文书工作。      
然后，国家科学基金会指示，互联网域名注册的管理将由商业的第三方实体处理。        
InterNIC成立于1993年，与NSF合作，由Network Solutions，Inc.，General Atomics和AT＆T组成。     
由于性能问题，通用原子公司合同在几年后被取消。     

**20世纪的WHOIS服务器非常宽容，可以进行通配符搜索。**            
WHOIS对某个姓氏的查询即可查询到所有该姓氏的所有个人的相关信息.              
具有给定关键字的查询返回包含该关键字的所有注册域名。给定管理联系人的查询返回了与管理员关联的所有域。          
**自从互联网商业化，多注册商和不道德的垃圾邮件发送者出现以后，这种相对宽松的查询环境就不复存在了。**                

在1999年12月1日，顶级域名（TLD）com，net和org的管理权被分配给了ICANN。             
此时，ICANN将这些TLD统一转换为精简的WHOIS模型。同时现存的WHOIS客户端当时停止工作。      
一个月后，它具有自我检测的通用网关接口支持，以便同的程序可以运行基于W相eb的WHOIS查询，     
以及基于请求的TLD支持多个WHOIS服务器的外部TLD表。**这最终成为现代WHOIS客户端的规范模型。**     

到了2005年，与二十世纪八十年代初期相比，出现了更多的通用顶级域名,国家码顶级域名。     
这导致域名注册商和注册商协会的关系网络变得更为复杂，特别是随着互联网基础设施的管理越来越国际化。        
因此，**在网络上执行WHOIS查询已知并使用正确，权威的WHOIS服务器**。执行WHOIS代理搜索的工具已经很普遍。        


### WHOIS历史 ICANN 自述
来源 : https://whois.icann.org/en/history-whois

#### WHOIS的历史

WHOIS的历史可以追溯到1982年，当时互联网工程任务组发布了针对ARPANET用户的目录服务协议。     
最初，该目录简单列出了通过ARPANET传输数据的任何人所要求的联系信息。       

随着互联网的发展，WHOIS开始服务于域名注册人，执法人员，知识产权和商标所有者，企业和个人用户等不同利益相关者的需求。        
但协议仍然基于原始的IETF标准。这是ICANN组织在1998年成立时继承的WHOIS协议。            

2009年9月30日，ICANN与美国商务部签署了“承诺书确认书”（AOC），承认ICANN为独立，私人和非营利性的组织。       
随着2016年向新的ICANN章程过渡，最初由过期的AOC建立的WHOIS义务被新的gTLD注册目录服务（RDS）义务所取代。     

根据现有的共识性政策和合同，ICANN将继续致力于“遵守适用的法律，执行其现有的有关WHOIS的政策。”这样的现行政策要求ICANN采取措施，     
及时，不受限制地公开访问准确完整的WHOIS信息，包括域名注册者,技术支持和管理的联系信息。“      
此外，在新的ICANN章程下，还将继续针对WHOIS政策定期审核的具体规定。           

在1999年，ICANN开始允许其他实体提供域名注册服务。注册管理机构负责维护顶级域名的注册管理机构。     

多年来，互联网名称与数字地址分配机构（ICANN）已经与注册服务商和注册管理机构达成协议，修改了WHOIS服务要求。      
这些协议建立了规定如何运行WHOIS服务的基本框架。此外，ICANN已经通过并实施了多项旨在改善WHOIS服务的共识性政策：      

* **WHOIS数据提醒政策（2003年）**：注册服务机构至少每年至少一次向所有域名注册人发送电子邮件，并提醒他们检查和更新其WHOIS数据; 例如，在新的手机号码或更改的业务地址的情形下。
* **“还原名称准确性政策”（2004）**：如果域名由于包含不正确的联系人数据而被删除，或者对信息请求没有响应，则域名必须保留，直到域名注册人提供更新且准确的WHOIS数据。
* **WHOIS营销限制政策（2004年）**：此政策对注册服务商认证协议进行了两处更改，试图禁止使用WHOIS数据进行市场营销和重新使用。     
注册服务商必须要求第三方“同意不使用[WHOIS]数据来允许，启用或以其他方式支持任何营销活动”和“不出售或重新分配[WHOIS]数据”（有一些例外）。

此外，ICANN继续采用新的共识性政策来改进现有的WHOIS服务。目前正在实施的政策包括：

* **.COM，.NET和.JOBS（2014）的'thick' RDDS（WHOIS）过渡政策**：该政策解决了“thin”和“thick”WHOIS注册管理机构之间的差异，要求将剩余的“thin”注册管理机构转换为“thick”数据模型。
* **其他WHOIS信息政策（2014）**：此政策要求注册商和注册管理机构将信息纳入WHOIS输出中，以帮助用户更好地识别域名注册的发起注册服务商并了解域名注册的状态代码。
* **隐私和代理服务认证政策（2015）**：本政策涉及到一些域名注册人所使用的隐私和代理服务认证相关问题，以保持有关他们的某些信息不会在WHOIS中发布。
* **联系信息政策的翻译和音译（2015年）**：该政策涉及国际化注册数据如何收集和显示在注册数据目录服务中，以便将这些数据翻译和/或音译为其他语言和/或脚本。
* **注册管理机构注册数据目录服务一致标记和显示策略（2017年更新）**：该政策要求不同注册管理机构显示的WHOIS输出保持一致。

最后，ICANN组织与注册管理机构和注册服务机构合作审查和更新与WHOIS政策实施有关的适当程序，例如：

* **审查现有的ICANN处理Whois与隐私法律冲突的程序（2016）**
* **WHOIS 数据保留规范豁免（2013）**

WHOIS是ICANN和其他互联网管理机构以及全球互联网社区长期争论和研究的中心。       
互联网生态系统的发展为WHOIS在各个领域带来了挑战：准确性，访问，合规性，隐私，滥用和欺诈，成本和警务。       
WHOIS的基本设计出现了一些问题，许多人认为这不足以满足当今互联网的需求，更不用说未来的互联网。       
对WHOIS过时的担忧与对更换或替换WHOIS所涉及的成本的担忧相等。

**WHOIS面临着这些挑战，因为它的使用范围超出了创始协议设计时的设想。**     
更多的利益相关者以合法的方式利用它的创造者所无法预见的。因此**ICANN多年来不得不修改WHOIS**;       
关于准确性的共识性政策就是一个主要的例子，以及在注册商认证协议（2013 RAA）的新形式中引入验证和验证要求。

WHOIS还面临其他挑战。**由于域名已经成为打击欺诈和滥用行为的重要武器**，ICANN的安全与稳定咨询委员会在SAC第38号建议：     
**注册服务机构滥用联络点建议注册服务商和注册管理机构公布滥用联系人信息**。     
这个滥用联系人将负责处理和提供从其他注册管理机构，注册服务机构，执法机构和反滥用社区的公认成员等认可方面收到的滥用投诉的及时回应。       
2014年，2013 RAA下的注册商需要发布WHOIS数据，其中包括注册商滥用联系人。

即使进行了这些修改，也有社区呼吁改进当前的WHOIS模型。互联网名称与数字地址分配机构（ICANN）的通用名称支持组织（GNSO）将探讨这些领域，       
并努力制定新政策，以酌情解决每个问题。在过去的十年中，GNSO已经开展了一系列重新评估当前WHOIS系统的活动，并试图收集检查WHOIS对利益相关方重要性的数据。       
应理事会的要求，ICANN组织启动了一系列WHOIS研究：

**WHOIS隐私和代理服务滥用** - 本研究调查了通过隐私或代理服务注册通用顶级域名（gTLD）域名以进行涉嫌非法或有害的互联网活动的程度，        
以掩盖犯罪人的身份。国家物理实验室在2014年3月进行了这项研究并交付了结果。

**WHOIS注册人识别** - 本研究使用WHOIS数据和与域名相关的内容对注册gTLD域名的实体进行分类，     
包括自然人，法人，隐私和代理服务提供商。使用相关的Internet内容; 然后使用这些域名和潜在的商业活动对实体进行分类。       
芝加哥大学的NORC进行了这项研究，并于2013年5月交付了结果。       

**WHOIS滥用** - 本研究调查了公共WHOIS数据被滥用于处理有害通信如网络钓鱼或身份盗用的程度。               
美国宾夕法尼亚州匹兹堡市的卡内基梅隆大学的Cylab进行了这项研究，并于2013年12月交付了结果。         

**WHOIS隐私和代理中继和显示** - 本研究评估了对使用代理和隐私服务注册的通用中继和身份揭示请求进行深入研究的可行性。     
Interisle Consulting Group在美国马萨诸塞州波士顿进行了这项研究，并于2012年6月交付了结果。        

**WHOIS服务要求调查** - 本研究调查了社区成员对WHOIS服务要求达成一致的程度。      
GNSO工作组于2010年7月召开了调查并交付了结果。

关于**域名WHOIS术语和结构的报告** - 为了澄清关于WHOIS术语各种含义的混淆，SSAC进行了这项研究。       
该报告于2011年9月发布，建议ICANN过渡到采用新术语来指定WHOIS的不同方面。因此，ICANN采用了新的术语来提及WHOIS系统的各个方面，其中包括：

* **域名注册数据** -是指域名注册人注册域名时提供和注册服务商或注册收集的信息。
* **域名注册数据访问协议** - 指的是通信交换的元素 - 查询和响应 - 可以访问注册数据。例如，WHOIS协议（RFC 3912）和超文本传输协议（HTTP）（RFC 2616及其更新）通常用于提供公共接入。
* **域名注册数据目录服务** - 指的是由注册管理机构和注册商提供的访问域名注册数据的服务。这个术语现在经常与注册目录服务（RDS）互换使用。

2013年，第一个WHOIS审核小组（WHOIS RT）提出了一系列建议，以改进当时ICANN组织监督WHOIS系统的方式。      
这些改进措施包括开发新的准确性报告系统（ARS），主动识别不准确的WHOIS记录，并将其转发给注册服务机构进行跟踪，以提高数据准确性并创建准确度度量标准。       

同样在2013年，ICANN成立了一个gTLD目录服务专家工作组（EWG），负责设法打破ICANN社群在WHOIS系统的实用性和命运方面的僵局。        
在其最终报告（2014年）中，EWG建议将模式转变为“下一代RDS，仅收集，验证和披露gTLD注册数据仅用于允许的目的。        
虽然基本数据将保持公开可用，认可的请求者，他们表明自己，陈述他们的目的，并同意追究适当的使用责任。

最近更新：2017年7月

### 相关资料，网站
##### RFC 协议  
https://tools.ietf.org/

##### ICANN 官网
https://www.icann.org/

##### ICANN的CZDS服务
https://czds.icann.org/en

##### IANA 官网        
https://www.iana.org/

##### 最权威的TLD与WHOIS服务器映射关系(IANA)        
http://www.iana.org/domains/root/db

##### 较好的第三方WHOIS查询工具
https://who.is/
https://research.domaintools.com/
https://whois.icann.org/en

##### 较好的第三方WHOWAS查询工具
https://www.benmi.com/

## WHOIS 的过去
#### CRISP和IRIS 
2003年，IETF委员会成立，为查询域名和网络号码信息创建了一个新的标准：交叉注册信息服务协议（CRISP）。
从2005年1月到2006年7月，这个提议的新标准的工作名称是互联网注册管理机构信息服务（IRIS) IRIS的初始IETF建议标准RFC是：

* RFC 3981 - IRIS：互联网注册信息服务（IRIS）核心协议
* RFC 3982 - IRIS：互联网注册信息服务（IRIS）的域名注册（垃圾）类型
* RFC 3983 - 通过块可扩展交换协议（BEEP）使用Internet注册信息服务（IRIS）        
* RFC 4992 - 用于块注册表信息服务的XML流水线
* RFC 5114 - 用于Internet注册信息服务（IRIS）的域可用性检查（DCHK）注册表类型

*注意：IETF CRISP工作组不应与同名“统一RIR IANA管理权建议团队”（CRISP团队）号码资源组织（NRO）团队混淆。[*
*具体协议内容见文档*

#### RFC 812&945

* RFC 812 - NICNAME/WHOIS
* RFC 954 - NICNAME/WHOIS

*具体协议内容见文档*
## WHOIS 的现在

* **RFC 3912**

### RFC 3912 关键内容摘要

##### 1.  介绍

  WHOIS一个是基于TCP的面向事务的查询/响应协议       
  其广泛被应用于向互联网用户提供信息查询服务       
  虽然最初用来提供“白页”服务和有关注册域名的信息      
  但是当前的部署涵盖了内容了更广泛的信息服务。   
  该协议以可读格式传送其内容。本文件更新了        
  规范WHOIS协议，从而废除RFC 954 [1]。  

  由于历史原因，WHOIS缺乏很多协议设计属性,         
  例如国际化和强壮安全性，这可以从最近设计的IETF协议中预料到。        
  本文不会尝试纠正任何这些缺点。相反，这份备忘录     
  如是记录了WHOIS协议的情况。在某些地方       
  本文确实记录了一些WHOIS协议的众所周知的缺点。       
  有关于协议可能带来的新的功能与更新所带来的缺陷的相关讨论,       
  正在单独的IETF活动中处理（CRISP 工作小组）。     


##### 2.  协议规范

  WHOIS服务器在TCP端口43上侦听来自WHOIS客户端的请求。      
  WHOIS客户端向WHOIS服务器发送文本请求,然后      
  WHOIS服务器以文本内容回应。所有的请求都是     
  以ASCII码<CR>接ASCII码<LF>结尾。回应可能       
  包含多行文本，所以存在ASCII码<CR>或      
  ASCII码<LF>字符不表示响应结束。该响应输出完成后，     
  WHOIS服务器立即关闭与WHOIS客户端的连接。       
  关闭的TCP连接是对客户端的指示回应已收到。      

##### 3.  协议样例

  如果有人向位于whois.nic.mil的WHOIS服务器请求     
  有关"Smith"的信息,在网络上传送的数据包将会像是这样:      

    ```
    WHOIS客户端                位于 whois.nic.mil 的WHOIS服务器 

    打开 TCP      ---- (SYN) ------------------------------>
                <---- (SYN+ACK) -------------------------
    发送查询    ---- "Smith<CR><LF>" -------------------->
    获得响应    <---- "有关于 Smith 的信息<CR><LF>" ---------
                <---- "更多有关于 Smith 的信息<CR><LF>" ----
    关闭          <---- (FIN) ------------------------------
                ----- (FIN) ----------------------------->
    ```

##### 4.  国际化

  WHOIS协议尚未国际化。 WHOIS     
  协议没有指示正在使用的字符集的机制。      
  最初，主要使用的文本编码是US-ASCII。在     
  实际中，一些WHOIS服务器，尤其是美国境外的服务器，     
  可能会使用其他字符集来解析请求或发出回应。      
  无法预测或表示的文本编码了对此WHOIS协议的     
  的互通性(当然,也包括可用性)有着不利的影响.     


##### 5.  安全性考虑

  WHOIS协议没有强有力的安全措施。WHOIS协议       
  缺乏有关访问控制，完整性和机密性的机制。        
  因此，基于WHOIS的服务只能用于非敏感的信息     
  并准备让所有人都可以访问。      
  此项安全机制的缺失意味着在本协议编写时
  通常可能不会被IETF所接受 


### 现行WHOIS服务器的重要缺陷
基于RFC 3912,我们可以预见现行的WHOIS协议及服务存在着如下缺陷:

* 尚未统一标准的编码
* 缺乏访问控制
* 对于WHOIS数据没有验证正确性的机制
* 对于越来越多的顶级域与WHOIS服务器缺乏统一的,完善的规范与标准


### 对于现行WHOIS的批评
对WHOIS的批评之一是**缺乏对数据的全面访问。很少有组织和个人可以实时访问完整的数据库**。        
其他人则认为**域名注册信息完全暴露**，尽管域名隐私服务可以大大缓解这个问题。        
目前互联网名称与数字地址分配机构（ICANN）普遍要求提供邮编,地址,电话号码和电子邮件地址              
任何查询WHOIS服务器的人都可以轻松访问注册人（域名所有者）的详细联系信息，例如地址和电话号码。但是，        
**该政策可以使垃圾邮件发送者，直销商，身份盗窃者或其他攻击者掠夺目录中的个人信息**。        
尽管互联网名称与数字地址分配机构（ICANN）一直在探索改变WHOIS以实现更高的隐私性，但主要利益相关者之间缺乏共识，应该进行什么样的更改。     
一些域名注册商提供私人注册（也称为域名隐私），显示注册商的联系信息，而不非注册这本人的。随着许多注册商开始提供私人注册服务，相关风险已经被降低。

研究表明，**垃圾邮件发送者可以收集来自WHOIS服务器的纯文本电子邮件地址。**
出于这个原因，**一些提供WHOIS查询的WHOIS服务器和网站已经实施了限速系统，**             
**例如基于网络的CAPTCHA和每个用户IP地址的有限数量的搜索查询。**

WHOIS协议不是以全世界用户为中心的。**WHOIS服务器和/或客户端无法确定对查询或数据库内容有效的文本编码**。             
许多服务器最初使用的是US- ASCII，直到很久以后才考虑到国际化问题.这可能会影响美国以外国家WHOIS协议的可用性或有用性。       
在国际化的情况下，客户端应用程序有责任在其本地语言脚本和punycode中的DNS名称之间执行域名转换。        

## WHOIS 的未来

### ICANN提议废除WHOIS     
互联网名称与数字地址分配机构（ICANN）的专家工作组（EWG）于2013年6月24日建议**应废止WHOIS**。          
它建议将WHOIS替换为一个保持绝大多数互联网用户的信息的系统，并且只为“允许的目的”披露信息。             

专家工作组收集了初步报告中的公众意见，直至2013年9月13日。其最终报告于2014年6月6日发布，对建议没有任何有意义的修改。     
ICANN现在处于“重新发明WHOIS的过程”，正在从事“ICANN WHOIS Beta”的工作。      

#### CNNIC技术专家主导制定互联网下一代WHOIS国际标准
来源: http://www.cac.gov.cn/2015-03/31/c_1114815085.htm
2015年3月26日，在美国达拉斯召开的国际互联网工程任务组（Internet Engineering Task Force，简称IETF）第92次大会上传来消息，      
由CNNIC技术专家参与制定的三篇下一代WHOIS协议文稿正式发布成为IETF国际标准，分别命名为RFC7480、RFC7481和RFC7485。       
这是我国技术人员首次参与制定的互联网域名系统基础协议相关的推荐类型国际标准，      
此次标准的发布意味着提供全球互联网域名及IP地址注册信息查询这一基础性功能的WHOIS服务将迈入崭新时代，       
未来可为全球网民提供更为便捷和安全的WHOIS服务体验。

现有的WHOIS协议（RFC3912）是2004年由IETF制定发布，是用于查询互联网域名及IP地址相关注册信息的重要基础性协议。               
2012年5月，CNNIC联合ICANN、Verisign等国际机构，针对现有协议暴露出缺乏国际化支持机制、缺乏数据扩展机制、缺乏安全隐私保护机制等诸多问题              
而成立专项工作组，推动制订下一代WHOIS协议。CNNIC技术专家孔宁博士作为该工作组核心设计小组的专家成员，             
与国际上其他技术专家历时三年完成下一代WHOIS系列国际标准的制定工作。                
其中，RFC7485是由CNNIC技术专家周琳琳作为第一作者主导制定。     
RFC7480和RFC7481属于推荐标准类型，由孔宁博士与国际技术专家合作完成，此类型国际标准发布后，将获得业界广泛支持与应用。       

多年来，CNNIC致力推动互联网基础资源相关国际标准的制定工作。本次CNNIC参与制定的三项IETF国际标准，     
是继国际化域名、国际化多语种电子邮件地址相关国际技术标准之后，在互联网域名系统基础协议国际技术标准领域中的又一突破。      
至此，CNNIC已经参与制定了10项IETF国际标准。与此同时，CNNIC积极在国际社群中参与互联网基础资源相关技术研发工作。     
2012年10月，CNNIC成功中标互联网名字与编号分配机构（ICANN）下一代WHOIS系统开源项目，伴随着下一代WHOIS协议国际标准的发布，           
由CNNIC研发的下一代WHOIS系统开源软件也将成为全球互联网域名行业的重要基础软件。CNNIC主任李晓东研究员表示，        
我国技术专家深入参与互联网国际标准制定，将有力推动我国发展下一代安全可信互联网的进程，     
促进我国互联网域名行业在迈入NewgTLD（新通用顶级域）时代发展中占据主动地位，并对进一步提升我国在国际互联网社群的影响力具有积极意义。

### 下一代WHOIS协议：RDAP
WHOIS协议系统是用于查询域名是否被注册，以及注册相关的详细信息的系统。       
这个老旧的WHOIS协议将会被新的RDAP协议取代。      

现有的WHOIS协议（RFC3912）是2004年由IETF制定发布，是用于查询互联网域名相关注册信息的重要基础性协议。        

2012年5月，CNNIC联合ICANN、Verisign等国际机构，     
针对现有协议暴露出缺乏国际化支持机制、缺乏数据扩展机制、缺乏安全隐私保护机制等诸多问题而成立专项工作组，推动制订下一代WHOIS协议。

下一代WHOIS协议即RDAP （Registration Data Access Protocol，注册数据访问协议）            
于2015年3月26日正式发布为IETF RFC国际技术标准（包括：RFC7480、RFC7481、RFC7482、RFC7483、RFC7484、RFC7485），     
该协议主要支持域名、IP地址、AS号、名字服务器以及实体的查询，其中域名、名字服务器和实体可以支持搜索功能。      
此外，还可支持IDN域名查询和搜索、查找WHOIS服务器的重定向、认证和数据访问权限三项具体功能。       

#### WEIRDS和RDAP
2013年，IETF承认IRIS并不是WHOIS的成功替代品。主要的技术原因似乎是IRIS的复杂性。      
此外，非技术性原因被认为是IETF不通过判决的地方。同时，ARIN和RIPE NCC通过RESTful Web服务设法为WHOIS数据提供服务。        
该章程（2012年2月起草）规定了单独的规范，首先为号码注册管理机构和名称注册管理机构遵循。工作组提出了五项提议的标准文件和一个信息文件：      

* RFC 7480 - 注册数据访问协议（RDAP）中的HTTP使用
* RFC 7481 - 注册数据访问协议（RDAP）的安全服务
* RFC 7482 - 注册数据访问协议（RDAP）查询格式
* RFC 7483 - 注册数据访问协议（RDAP）的JSON响应
* RFC 7484 - 查找权威注册数据（RDAP）服务
* RFC 7485 - WHOIS注册对象的清单和分析

### 参考资料
[RFC 协议](https://tools.ietf.org/rfc/)       
[wikipedia - WHOIS](https://en.wikipedia.org/wiki/WHOIS)        
[ICANN](https://www.icann.org/)     


## Contact
H-J-13(@`13)                                         
z.g.13@163.com/h.j.13.new@gmail.com                 
Harbin Institute of Technology at Weihai     

[`13 Blog](http://houjie13.com/)  

[`13的博客](http://www.jianshu.com/u/75156f101757)