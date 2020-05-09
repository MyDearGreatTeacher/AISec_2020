# 20200517
```
漏洞評鑑系統(CVSS) :羅報告

https://ithelp.ithome.com.tw/articles/10203313
https://secbuzzer.co/post/106


漏洞評鑑系統(Common Vulnerability Scoring System；CVSS) 由美國國家基礎建設諮詢委員會 (NIAC) 委託製作，
是一套公開的評鑑標準，經常被用來評比企業資訊科技系統的安全性，並受到eBay、賽門鐵克(Symantec)、思科(Cisco)、甲古文(Oracle)等眾多軟體廠商支援。
由於CVSS是運用數學方程式來判定某特定網路的安全性是否存在弱點，普遍被認為較具中立性。

CVSS的判定標準，不但包含威脅的嚴重性，遠端網路是否能遙控資安漏洞、利用網路弱點，攻擊者是否需要登入才會產生威脅等等，都被列入評比。

CVSS的評分分數從0分到10分，0代表沒有發現弱點，而10則代表最高風險。
https://www.digitimes.com.tw/tech/dt/n/shwnws.asp?cnlid=10&id=0000100727_WBC8XRHR1Y3H1O8HWCHDQ

Common Vulnerability Scoring System Version 3.0 Calculator
https://www.first.org/cvss/calculator/3.0#CVSS:3.0/AV:N/AC:H/PR:L/UI:N/S:U/C:H/I:H/A:H

以8個面向來進行評分，並得出一個0.0～10.0分的分數，分數越高代表漏洞危險程度越高：

攻擊向量 (Attack Vector, AV)
Network (N)：由網際網路網路進行攻擊
Adjacent (A)： 由受限制的網路進行攻擊，如區域網路及藍芽等
Local (L)：在不連接網路的狀況下進行攻擊
Physical (P)：需接觸到實體機器才能進行攻擊
攻擊複雜度 (Attack Complexity, AC)
Low (L)：低，攻擊可被輕易重現
High (H)：高，須由攻擊者達成數項條件後才能成功
是否需要提權 (Privileges Required, PR)
None (N)：不需要
Low (L)：需要一般使用者權限
High (H)：需要管理者權限
是否需要使用者操作 (User Interaction, UI)
None (N)：不需要
Required (R)：需要使用者操作某些動作才能讓攻擊成功
影響範圍 (Scope, S)
Unchanged (U) ：僅影響含有漏洞的元件本身
Changed (C)：會影響到含有漏洞的元件以外的元件
機密性影響 (Confidentiality, C)
None (N)：無影響
Low (L)：攻擊者可以取得機密資料，但無法使用該資料
High (H)：攻擊者可以取得機密資料，且可以使用該資料
完整性影響(Integrity, I)
None (N) ：無影響
Low (L) ：攻擊者有部分權限以竄改某些資料，對含有漏洞之元件影響較小
High (H)：攻擊者有權限竄改所有資料，對含有漏洞之元件有嚴重影響
可用性影響 (Availability, A)
None (N)：無影響
Low (L)：可用性受到影響，導致服務或元件仍可被部分取得，或是時好時壞
High (H)：可用性受到嚴重影響，導致服務或元件完全不可被取得

舉個例子，WannaCry使用的漏洞CVE-2017-0144的CVSSv3分數是8.1，其中8項選項如下：
Attack Vector (AV): Network
Attack Complexity (AC): High
Privileges Required (PR): None
User Interaction (UI): None
Scope (S): Unchanged
Confidentiality (C): High
Integrity (I): High
Availability (A): High

如果想要試著玩看看各項排列組合產出的分數是多少，可以到FIRST網站上的CVSSv3計算機去試試看：https://www.first.org/cvss/calculator/3.0 。
系統也會根據你的選擇產出一個向量字串 (Vector String)，用於描述你對這個漏洞的各項選擇，例如CVE-2017-0144的向量字串長相則為「CVSS:3.0/AV:N/AC:H/PR:N/UI:N/S:U/C:H/I:H/A:H」，我們也可以看出來，這個字串是根據上述8個面向分別描述選擇的答案為何所產出的。
```

# AI_Sec_2020 課程內容
```
人工智慧
期中考
資訊安全
期末考
```
### 期中/末報告題目
```
1.論文相關
2.國內外碩士論文或經典論文
3.資訊安全實戰:  資訊安全測試
  vuln hub
  https://www.vulnhub.com/
  
  解答範本:
  
  [1]遠端卓面協定漏洞分析
  RDP Session Hijacking with tscon
  https://www.hackingarticles.in/rdp-session-hijacking-with-tscon/
  [2]Chatbot security
    Security Best Practices for Bot Builders
    https://www.slideshare.net/MaxFeldman4/security-best-practices-for-bot-builders
    根本是網站漏洞
```
### 資安測試主題
```
Web Shells Penetration Testing ===上傳惡意程式到網站  然後在執行此惡意程式
https://www.hackingarticles.in/web-shells-penetration-testing/

漏洞測試平台:
  [1]DVWA
  [2]使用PentesterLab:Web for Pentester平台
     https://pentesterlab.com/exercises/web_for_pentester/course

請參考報告範本
延伸建議:增加許多討論
一句話木馬
web shell 程式分析
```
```
PentesterLab:Web for Pentester平台安裝與測試
[1]安裝
   web for pentester lab 1&2 installation in virtual box in linux
   https://www.youtube.com/watch?v=Njrt5aRswOc
[2]解答
   Web For Pentester - SQL Injection 1
   https://www.youtube.com/watch?v=w1LHfGiHmYs
```
```
攻擊HTTP Authentication(認證)的各種技巧
Multiple Ways To Exploiting HTTP Authentication
https://www.hackingarticles.in/multiple-ways-to-exploiting-http-authentication/

學習目標:
1.熟悉HTTP Authentication基本觀念
2.熟悉HTTP Authentication的設定技術
3.熟悉HTTP Authentication的各種攻擊技術

Exploiting HTTP Authentication
xHydra
Hydra
Ncrack
Medusa
Metasploit
Burp Suite
```
```
Multiple Ways to Crack WordPress login
攻擊WordPress網站的登入===猜帳號與密碼
https://www.hackingarticles.in/multiple-ways-to-crack-wordpress-login/

暴力攻擊
測試環境建置
三種實戰案例
如何避免暴力攻擊的成功 How to avoid a Brute Force attack?
```
```
使用docker技術建置各種網站測試平台

https://www.hackingarticles.in/web-application-pentest-lab-setup-using-docker/

git clone https://github.com/eystsen/pentestlab.git
cd pentestLab
./pentestLab.sh --help
```
### MalwareAnalysisForHedgehogs
```
https://www.youtube.com/channel/UCVFXrUwuWxNlm6UNZtBLJ-A
```
```
Malware Analysis - Dumping COVID-19.jar RAT with Java Instrumentation
觀看次數：820次•2020年4月25日
https://www.youtube.com/watch?v=QAzs66psLjY&feature=em-uploademail
```
```
Malware Analysis - Unpacking NetWiredRC With DnSpy
觀看次數：1,788次•2016年7月10日
https://www.youtube.com/watch?v=dLIbkg_8O68
```
### 期中報告題目
```

```
# 20200425
```
人工智慧tensorflow影像辨識

Image classification
https://www.tensorflow.org/tutorials/images/classification
```
# 參考書與教科書
```
https://github.com/MyDearGreatTeacher/AI4ALL
```
# 資訊安全主題
### PT: LINUX Server滲透測試實戰 20200418
```
VSFTPD v2.3.4 Backdoor Command Execution
https://www.youtube.com/watch?v=6XHrF4x_0i0

https://www.rapid7.com/db/modules/exploit/unix/ftp/vsftpd_234_backdoor

VSFTPD v2.3.4 Backdoor Command Execution 简易分析
http://wp.blkstone.me/2019/08/vsftpd-v2-3-4-backdoor-command-execution-brief-analysis/
```
```
nmap指令參數
https://blog.gtwang.org/linux/nmap-command-examples-tutorials/
```
# 人工智慧
```
Python程式
   https://github.com/HappyHackingHigh/HappyPythonDay/tree/master/python
資料分析:NUMPY   Matplotlib   PANDAS
機器學習:
深度學習:
```
# 資料分析:NUMPY   Matplotlib   PANDAS
```
https://github.com/MyDearGreatTeacher/AI4ALL/tree/master/資料分析
```

##  機器學習實戰練習
```

```

## 深度學習實戰練習
```

```

#
