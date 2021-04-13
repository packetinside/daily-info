# 互联网安全 推荐
| ts | title | url| 
| --- | --- | ---| 


# 玄武实验室 推荐
| ts | title | url| 
| --- | --- | ---| 
| 20210413 | CVE-2021-29627：由于 FreeBSD 的 accept_filter 处理程序错误而留下一个空指针，可能被利用于内核提权。 | https://github.com/raymontag/cve-2021-29627| 
| 20210413 | Process Herpaderping：通过在映像映射后修改磁盘上的内容来掩盖进程意图的方法。 | https://movaxbx.ru/2021/04/11/process-herpaderping/| 
| 20210413 | Chrome 和Firefox 等浏览器的 WebDriver REST APIs RCE 分析。 | https://starlabs.sg/blog/2021/04/you-talking-to-me/| 
| 20210413 | SSRF 漏洞可能的攻击方式列表。 | https://github.com/assetnote/blind-ssrf-chains| 
| 20210413 | 介绍为什么 macOS EDR（Endpoint Detection and Response）不应该运行在 Rosetta 2 下。 | https://www.sentinelone.com/blog/why-your-macos-edr-solution-shouldnt-be-running-under-rosetta-2/| 
| 20210413 | PD Actions：使用 GitHub Actions 实现自动化的安全工作流程。 | https://blog.projectdiscovery.io/github-actions-for-application-security/| 
| 20210413 | 在 Tesla Model 3 上利用 CVE-2020-6418。 | https://leethax0.rs/2021/04/ElectricChrome/| 
| 20210413 | 关于内核漏洞的原理分析。 | http://www.yuque.com/posec/public/sp9bs1| 


# 安全维基 推荐
| ts | title | url| 
| --- | --- | ---| 
| 20210413 | 微信小程序反编译 | https://www.sec-in.com/article/1012| 
| 20210413 | 从BCTF人机对抗视角浅谈自动化攻防技术发展 | https://mp.weixin.qq.com/s/5wR37FLoTPn3fftxZw_Brw| 


# CVE Github 推荐
| ts | cve_id | title | url | cve_detail| 
| --- | --- | --- | --- | ---| 
| 20210413T11:51:21Z | cve-2021-29627 | Trigger-only for CVE-2021-29627 | https://github.com/raymontag/cve-2021-29627 | In FreeBSD 13.0-STABLE before n245050, 12.2-STABLE before r369525, 13.0-RC4 before p0, and 12.2-RELEASE before p6, listening socket accept filters implementing the accf_create callback incorrectly freed a process supplied argument string. Additional operations on the socket can lead to a double free or use after free.| 
| 20210413T11:44:17Z | CVE-2020-17519 | CVE-2020-17519 Cheetah | https://github.com/givemefivw/CVE-2020-17519 | A change introduced in Apache Flink 1.11.0 (and released in 1.11.1 and 1.11.2 as well) allows attackers to read any file on the local filesystem of the JobManager through the REST interface of the JobManager process. Access is restricted to files accessible by the JobManager process. All users should upgrade to Flink 1.11.3 or 1.12.0 if their Flink instance(s) are exposed. The issue was fixed in commit b561010b0ee741543c3953306037f00d7a9f0801 from apache/flink:master.| 
| 20210413T09:07:38Z | CVE-2021-6666 | Null | https://github.com/givemefivw/CVE-2021-6666 | 未查询到CVE信息| 
| 20210413T07:51:29Z | CVE-2021-24086 | Proof of concept for CVE-2021-24086, a NULL dereference in tcpip.sys triggered remotely. | https://github.com/0vercl0k/CVE-2021-24086 | Windows TCP/IP Denial of Service Vulnerability| 
| 20210413T07:12:14Z | CVE-2020-5902 | Auto exploit RCE CVE-2020-5902  | https://github.com/haisenberg/CVE-2020-5902 | In BIG-IP versions 15.0.0-15.1.0.3, 14.1.0-14.1.2.5, 13.1.0-13.1.3.3, 12.1.0-12.1.5.1, and 11.6.1-11.6.5.1, the Traffic Management User Interface (TMUI), also referred to as the Configuration utility, has a Remote Code Execution (RCE) vulnerability in undisclosed pages.| 
| 20210413T04:26:27Z | CVE-2021-26832 | Cross Site Scripting (XSS) at the "Reset Password" page form of Priority Enterprise Management System v8.00 allows attackers to execute javascript on behalf of the victim by sending a malicious URL or directing the victim to a malicious site. | https://github.com/NagliNagli/CVE-2021-26832 | 未查询到CVE信息| 
| 20210413T01:07:21Z | cve-2020-2021 | Null | https://github.com/givemefivw/cve-2020-2021 | When Security Assertion Markup Language (SAML) authentication is enabled and the %Validate Identity Provider Certificate% option is disabled (unchecked), improper verification of signatures in PAN-OS SAML authentication enables an unauthenticated network-based attacker to access protected resources. The attacker must have network access to the vulnerable server to exploit this vulnerability. This issue affects PAN-OS 9.1 versions earlier than PAN-OS 9.1.3; PAN-OS 9.0 versions earlier than PAN-OS 9.0.9; PAN-OS 8.1 versions earlier than PAN-OS 8.1.15, and all versions of PAN-OS 8.0 (EOL). This issue does not affect PAN-OS 7.1. This issue cannot be exploited if SAML is not used for authentication. This issue cannot be exploited if the %Validate Identity Provider Certificate% option is enabled (checked) in the SAML Identity Provider Server Profile. Resources that can be protected by SAML-based single sign-on (SSO) authentication are: GlobalProtect Gateway, GlobalProtect Portal, GlobalProtect Clientless VPN, Authentication and Captive Portal, PAN-OS next-generation firewalls (PA-Series, VM-Series) and Panorama web interfaces, Prisma Access In the case of GlobalProtect Gateways, GlobalProtect Portal, Clientless VPN, Captive Portal, and Prisma Access, an unauthenticated attacker with network access to the affected servers can gain access to protected resources if allowed by configured authentication and Security policies. There is no impact on the integrity and availability of the gateway, portal or VPN server. An attacker cannot inspect or tamper with sessions of regular users. In the worst case, this is a critical severity vulnerability with a CVSS Base Score of 10.0 (CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:C/C:H/I:H/A:N). In the case of PAN-OS and Panorama web interfaces, this issue allows an unauthenticated attacker with network access to the PAN-OS or Panorama web interfaces to log in as an administrator and perform administrative actions. In the worst-case scenario, this is a critical severity vulnerability with a CVSS Base Score of 10.0 (CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:C/C:H/I:H/A:H). If the web interfaces are only accessible to a restricted management network, then the issue is lowered to a CVSS Base Score of 9.6 (CVSS:3.1/AV:A/AC:L/PR:N/UI:N/S:C/C:H/I:H/A:H). Palo Alto Networks is not aware of any malicious attempts to exploit this vulnerability.| 
| 20210413T01:05:46Z | cve-2020- | Null | https://github.com/givemefivw/cve-2020-tttt | 未查询到CVE信息| 
| 20210413T00:49:41Z | CVE-2021- | Null | https://github.com/givemefivw/CVE-2021-Finaltest | 未查询到CVE信息| 
| 20210413T00:46:22Z | CVE-2021- | Null | https://github.com/givemefivw/CVE-2021-Retest | 未查询到CVE信息| 


# klee on Github 推荐
| ts | title | url | stars | forks| 
| --- | --- | --- | --- | ---| 
| 20210413T08:46:44Z | Safe KLEE API for Rust | https://github.com/markhakansson/klee-rs | 0 | 0| 
| 20210413T08:27:10Z | Symbiotic is a tool for finding bugs in computer programs based on instrumentation, program slicing and KLEE | https://github.com/staticafi/symbiotic | 214 | 35| 
| 20210413T07:57:03Z | Raw bindings for KLEE | https://github.com/markhakansson/klee-bindings | 0 | 0| 
| 20210413T06:04:12Z | KLEE Symbolic Execution Engine | https://github.com/klee/klee | 1669 | 489| 
| 20210413T05:41:32Z | RVT is a collection of tools/libraries to support both static and dynamic verification of Rust programs. | https://github.com/project-oak/rust-verification-tools | 122 | 11| 


# s2e on Github 推荐
| ts | title | url | stars | forks| 
| --- | --- | --- | --- | ---| 


# exploit on Github 推荐
| ts | title | url | stars | forks| 
| --- | --- | --- | --- | ---| 
| 20210413T12:03:48Z | Open-Source Vulnerability Intelligence Center - Unified source of vulnerability, exploit and threat Intelligence feeds | https://github.com/Patrowl/PatrowlHearsData | 21 | 8| 
| 20210413T11:53:29Z | Null | https://github.com/oneoy/exploits1 | 0 | 0| 
| 20210413T11:42:49Z | Several tools for exploits. | https://github.com/vLeeH/protocol-tools | 0 | 0| 
| 20210413T11:36:27Z | Android RAT with web panel and undetectable App | https://github.com/Th30neAnd0nly/Ohm | 15 | 6| 
| 20210413T11:04:03Z | PS4 Exploit Host | https://github.com/Night-King-Host/Night-King-Host.github.io | 8 | 4| 
| 20210413T11:03:00Z | RGraph is an RDMA-assisted asynchronous distributed graph processing system. RGraph distributes edges into two parts to isolate master and mirror vertices. RGraph exploits the asymmetry of RDMA to accelerate the one-to-many communication between master and mirror vertices.  The results in comprehensive experiments show that compared to existing designs, PowerGraph, RGraph reduces the execution time by up to 81%. | https://github.com/CGCL-codes/RGraph | 4 | 4| 
| 20210413T10:35:52Z | CDK is an open-sourced container penetration toolkit, offering stable exploitation in different slimmed containers without any OS dependency. It comes with penetration tools and many powerful PoCs/EXPs helps you to escape container and takeover K8s cluster easily. | https://github.com/cdk-team/CDK | 1316 | 186| 
| 20210413T10:32:30Z | Null | https://github.com/luigifeola/CollectiveResourceExploitation | 0 | 0| 
| 20210413T10:04:53Z | Computer Network Exploitation (CNE) Field Manual | https://github.com/mzet-/z-field-manual | 2 | 2| 
| 20210413T09:54:01Z | Null | https://github.com/th3ken-dev/TH3KEN-EDITON | 2 | 0| 


# backdoor on Github 推荐
| ts | title | url | stars | forks| 
| --- | --- | --- | --- | ---| 
| 20210413T11:36:52Z | Null | https://github.com/BSalwiczek/backdoor-trojan | 0 | 0| 
| 20210413T10:25:32Z | Null | https://github.com/Bifrostbiolabs/Yggdrasil_Backdoor | 0 | 0| 
| 20210413T09:06:58Z | QA tasks for %Hidden Backdoors in Human-Centric Language Models% | https://github.com/HLori/Question-Answering | 0 | 0| 
| 20210413T06:06:55Z | A curated list of backdoor learning resources | https://github.com/THUYimingLi/backdoor-learning-resources | 209 | 34| 
| 20210413T04:18:07Z | 🤖An Evil and Smart Bot for Enslaving Windows. | https://github.com/wildonion/katyusha | 1 | 1| 
| 20210413T02:21:56Z | TrojanZoo provides a universal pytorch platform to conduct security researches (especially backdoor attacks/defenses) of image classification in deep learning. | https://github.com/ain-soph/trojanzoo | 60 | 10| 
| 20210413T01:57:07Z | A Simple android remote administration tool using sockets. It uses java on the client side and python on the server side | https://github.com/karma9874/AndroRAT | 202 | 92| 


# fuzz on Github 推荐
| ts | title | url | stars | forks| 
| --- | --- | --- | --- | ---| 
| 20210413T01:24:40Z | Digunakan untuk pengumpulan tugas PRAK. SCPK logika fuzzy | https://github.com/egaputra69/EgaErinovian_123190113_FuzzyLogic | 0 | 0| 
| 20210413T00:38:15Z | setup for fuzzing the Rust compiler | https://github.com/dwrensha/fuzz-rustc | 29 | 0| 
| 20210413T00:30:05Z | 📨 Responsive email template generator. | https://github.com/luangjokaj/fuzzymail | 114 | 4| 
| 20210413T00:06:40Z | OSS-Fuzz vulnerabilities for OSV. | https://github.com/google/oss-fuzz-vulns | 1 | 2| 



# 日更新程序
