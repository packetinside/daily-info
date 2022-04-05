# 互联网安全 推荐
| ts | title | url| 
| --- | --- | ---| 


# 玄武实验室 推荐
| ts | title | url| 
| --- | --- | ---| 


# 安全维基 推荐
| ts | title | url| 
| --- | --- | ---| 


# CVE Github 推荐
| ts | cve_id | title | url | cve_detail| 
| --- | --- | --- | --- | ---| 
| 20220405T12:11:32Z | CVE-2022-25636 | CVE-2022-25636 exploit rewritten with pipe primitive | https://github.com/veritas501/CVE-2022-25636-PipeVersion | | 
| 20220405T11:33:14Z | CVE-2022-22639 | Exploitation of CVE-2022-22639 | https://github.com/jhftss/CVE-2022-22639 | | 
| 20220405T11:26:16Z | CVE-2022-0185 | CVE-2022-0185 exploit rewritten with pipe primitive | https://github.com/veritas501/CVE-2022-0185-PipeVersion | | 
| 20220405T11:23:52Z | CVE-2021-22555 | CVE-2021-22555 exploit rewritten with pipe primitive | https://github.com/veritas501/CVE-2021-22555-PipeVersion | | 
| 20220405T11:20:31Z | CVE-2022-22947 | CVE-2022-22947 reproduce | https://github.com/aesm1p/CVE-2022-22947-POC-Reproduce | | 
| 20220405T08:56:16Z | CVE-2022-22963 | Null | https://github.com/darryk10/CVE-2022-22963 | | 
| 20220405T08:34:27Z | CVE-2020-24186 | CVE-2020-24186的攻击脚本 | https://github.com/Sakura-501/CVE-2020-24186-exploit | | 
| 20220405T02:59:59Z | CVE-2022-22965 | A Safer PoC for CVE-2022-22965 (Spring4Shell) | https://github.com/colincowie/Safer_PoC_CVE-2022-22965 | | 


# klee on Github 推荐
| ts | title | url | stars | forks| 
| --- | --- | --- | --- | ---| 
| 20220405T11:39:45Z | Imagine you could pick up a fragment of code in a complex system written in C and test it in separation on your Linux workstation without the burden of including all necessary headers and knowing the right set of #defines, compilation flags and the target architecture. Imagine you could use that code in a modern fuzzer or symbolic execution engine for thorough, focused deep testing.  AoT makes it possible to select a function from C code base and generate an executable off-target test harness. The harness can then be tested on a Linux machine, e.g. with ASAN, AFL or KLEE. The generated off-target is a self-contained binary and includes all the necessary types and definitions. In a nutshell, AoT makes it possible to test pieces of complex systems software in a unit test-like manner. What it is and how does this work?  First, you select a function F you are interested to test. AoT uses Code Aware Services (CAS) infrastructure, namely code database and compilation database to automatically pull in a subtree of functions called by F (that is, functions that F calls, functions that they call, etc.). By default, AoT stops at the module boundary: the functions compiled into the same module as F are pulled in, all the others are left out. For the functions that are left out AoT generates function stubs which can later be filled by the user. Such generated program is called an off-target, because it runs off the original code execution environment (e.g. a smartphone).  AoT works well with the AFL fuzzer (https://lcamtuf.coredump.cx/afl/) and the KLEE symbolic execution engine (http://klee.github.io/). It automatically generates binaries and test setup for those tools, so that you can start fuzzing the off-target immediately.  AoT is an automated solution that currently works in the human-in-the-loop model. It means that AoT tries to automate as much as possible, but a human operator is needed to fine-tune the results - e.g. provide stubs implementation or correct the program state initialization.  Potential uses of AoT are:      get a recursive list of functions given an entry point (could be used to get selective coverage)     get a list of types necessary for a given piece of code     instrument code for inter-structure fuzzing (unsupported yet)     instrument code for fuzzing / symbolic execution and apply those techiques to complex systems code     speed up development for slowly building targets (e.g. AOSP build process)  For example, let%s imagine we would like to test a message parser in a mobile phone modem. Normally, for such testing we need to set up the physical infrastructure, for example a base station that sends messages over the air to the mobile phone. When the message is received by the phone, the parser code is invoked. If there is an error, we need to collect potential crash logs (if any) and restart testing. The whole process is difficult to set up and a single testing cycle takes quite long. With AoT things look differently. We select the message parsing function as our target. AoT automatically pulls in the necessary definitions and functions compiled into the same module and generates function stubs for the functions outside of the module. Moreover, AoT generates the program state initialization and the code necessary for starting security fuzzing. The generated off-target code is self contained - we can compile it on a Linux box and use all standard tools such as fuzzers, gdb, sanitizers to test the code. As a result, we end up with a much faster setup and test cycle: the off-target generation takes minutes and we can re-execute the code up to thousands of times per minute. We can also easily attach a debugger and quickly inspect what went wrong.  As a further example let%s take the last point and let%s imagine we are modifying an AOSP kernel driver. Without AoT, we need to invoke entire build process to check if our change is correct. Moreover, we would need to run the code in an Android emulator or on the phone and find a way to invoke the changed driver code (which sometimes is not trivial). With AoT we can extract the code of the changed function and compile it within minutes. We can further use all available x86_64 Linux toolchains (gdb, sanitizers, etc.) to test it. As a result, the development & testing cycle should be much shorter. | https://github.com/Samsung/auto_off_target | 1 | 0| 
| 20220405T10:12:20Z | An open-source Chinese font derived from Fontworks% Klee One. 一款开源中文字体，基于 FONTWORKS 出品字体 Klee One 衍生。   | https://github.com/lxgw/LxgwWenKai | 5665 | 209| 
| 20220405T08:38:50Z | A concolic testing framework for RISC-V embedded software with support for SystemC peripherals | https://github.com/agra-uni-bremen/symex-vp | 6 | 1| 
| 20220405T06:06:08Z | KLEE Symbolic Execution Engine | https://github.com/klee/klee | 1931 | 550| 


# s2e on Github 推荐
| ts | title | url | stars | forks| 
| --- | --- | --- | --- | ---| 


# exploit on Github 推荐
| ts | title | url | stars | forks| 
| --- | --- | --- | --- | ---| 
| 20220405T12:11:32Z | CVE-2022-25636 exploit rewritten with pipe primitive | https://github.com/veritas501/CVE-2022-25636-PipeVersion | 3 | 1| 
| 20220405T11:57:51Z | An exploit primitive in linux kernel inspired by DirtyPipe | https://github.com/veritas501/pipe-primitive | 7 | 1| 
| 20220405T11:26:16Z | CVE-2022-0185 exploit rewritten with pipe primitive | https://github.com/veritas501/CVE-2022-0185-PipeVersion | 1 | 1| 
| 20220405T11:23:52Z | CVE-2021-22555 exploit rewritten with pipe primitive | https://github.com/veritas501/CVE-2021-22555-PipeVersion | 5 | 1| 
| 20220405T10:35:08Z | the ultimate exploits/references finder | https://github.com/ARPSyndicate/xlocate | 26 | 5| 
| 20220405T09:36:16Z | Search through Microsoft Security Bulletins (MSSB%s) to find relevant vulnerabilities and exploits to use against Windows target machines. | https://github.com/glowbase/windows-exploit-search | 0 | 0| 
| 20220405T09:00:47Z | Null | https://github.com/1337-L3V1ATH0N/OSCP-Win-Exploits | 0 | 0| 
| 20220405T08:49:32Z | 黑客工具收集仓库，包含主流和非主流漏洞利用工具，subdomain、备案查询工具、CVE仓库、Hacking Tools、Exploits、免杀工具、weblogic漏洞利用工具、Red Team、Cobalt Strike、C免杀、bypassAV、内网渗透工具、漏洞利用、工具插件、burpsuite插件； | https://github.com/CnHack3r/Awesome-hacking-tools | 47 | 8| 
| 20220405T08:46:11Z | 여러가지 Pwnable wargame exploit code | https://github.com/icaros7/pwnable_py | 0 | 0| 
| 20220405T08:34:27Z | CVE-2020-24186的攻击脚本 | https://github.com/Sakura-501/CVE-2020-24186-exploit | 0 | 0| 


# backdoor on Github 推荐
| ts | title | url | stars | forks| 
| --- | --- | --- | --- | ---| 
| 20220405T12:11:55Z | Linux eBPF backdoor over TCP. Spawn reverse shells, RCE, on prior privileged access. Less Honkin, More Tonkin. | https://github.com/kris-nova/boopkit | 302 | 27| 
| 20220405T08:22:16Z | Config files for my GitHub profile. | https://github.com/backdoorPhish/backdoorPhish | 0 | 0| 
| 20220405T06:46:12Z | A curated list of backdoor learning resources | https://github.com/THUYimingLi/backdoor-learning-resources | 453 | 87| 


# symbolic execution on Github 推荐
| ts | title | url | stars | forks| 
| --- | --- | --- | --- | ---| 
| 20220405T11:39:45Z | Imagine you could pick up a fragment of code in a complex system written in C and test it in separation on your Linux workstation without the burden of including all necessary headers and knowing the right set of #defines, compilation flags and the target architecture. Imagine you could use that code in a modern fuzzer or symbolic execution engine for thorough, focused deep testing.  AoT makes it possible to select a function from C code base and generate an executable off-target test harness. The harness can then be tested on a Linux machine, e.g. with ASAN, AFL or KLEE. The generated off-target is a self-contained binary and includes all the necessary types and definitions. In a nutshell, AoT makes it possible to test pieces of complex systems software in a unit test-like manner. What it is and how does this work?  First, you select a function F you are interested to test. AoT uses Code Aware Services (CAS) infrastructure, namely code database and compilation database to automatically pull in a subtree of functions called by F (that is, functions that F calls, functions that they call, etc.). By default, AoT stops at the module boundary: the functions compiled into the same module as F are pulled in, all the others are left out. For the functions that are left out AoT generates function stubs which can later be filled by the user. Such generated program is called an off-target, because it runs off the original code execution environment (e.g. a smartphone).  AoT works well with the AFL fuzzer (https://lcamtuf.coredump.cx/afl/) and the KLEE symbolic execution engine (http://klee.github.io/). It automatically generates binaries and test setup for those tools, so that you can start fuzzing the off-target immediately.  AoT is an automated solution that currently works in the human-in-the-loop model. It means that AoT tries to automate as much as possible, but a human operator is needed to fine-tune the results - e.g. provide stubs implementation or correct the program state initialization.  Potential uses of AoT are:      get a recursive list of functions given an entry point (could be used to get selective coverage)     get a list of types necessary for a given piece of code     instrument code for inter-structure fuzzing (unsupported yet)     instrument code for fuzzing / symbolic execution and apply those techiques to complex systems code     speed up development for slowly building targets (e.g. AOSP build process)  For example, let%s imagine we would like to test a message parser in a mobile phone modem. Normally, for such testing we need to set up the physical infrastructure, for example a base station that sends messages over the air to the mobile phone. When the message is received by the phone, the parser code is invoked. If there is an error, we need to collect potential crash logs (if any) and restart testing. The whole process is difficult to set up and a single testing cycle takes quite long. With AoT things look differently. We select the message parsing function as our target. AoT automatically pulls in the necessary definitions and functions compiled into the same module and generates function stubs for the functions outside of the module. Moreover, AoT generates the program state initialization and the code necessary for starting security fuzzing. The generated off-target code is self contained - we can compile it on a Linux box and use all standard tools such as fuzzers, gdb, sanitizers to test the code. As a result, we end up with a much faster setup and test cycle: the off-target generation takes minutes and we can re-execute the code up to thousands of times per minute. We can also easily attach a debugger and quickly inspect what went wrong.  As a further example let%s take the last point and let%s imagine we are modifying an AOSP kernel driver. Without AoT, we need to invoke entire build process to check if our change is correct. Moreover, we would need to run the code in an Android emulator or on the phone and find a way to invoke the changed driver code (which sometimes is not trivial). With AoT we can extract the code of the changed function and compile it within minutes. We can further use all available x86_64 Linux toolchains (gdb, sanitizers, etc.) to test it. As a result, the development & testing cycle should be much shorter. | https://github.com/Samsung/auto_off_target | 1 | 0| 
| 20220405T09:45:46Z | Angora is a mutation-based fuzzer.  The main goal of Angora is to increase branch coverage by solving path constraints without symbolic execution.  | https://github.com/AngoraFuzzer/Angora | 769 | 146| 
| 20220405T06:58:53Z | Playing with the VMProtect software protection. Automatic deobfuscation of pure functions using symbolic execution and LLVM. | https://github.com/JonathanSalwan/VMProtect-devirtualization | 530 | 94| 
| 20220405T06:06:08Z | KLEE Symbolic Execution Engine | https://github.com/klee/klee | 1931 | 550| 


# big4 on Github 推荐
| ts | title | url | stars | forks| 
| --- | --- | --- | --- | ---| 
| 20220405T05:38:58Z | Code for NDSS 2022 paper %MIRROR: Model Inversion for Deep Learning Network with High Fidelity% | https://github.com/njuaplusplus/mirror | 2 | 0| 


# fuzz on Github 推荐
| ts | title | url | stars | forks| 
| --- | --- | --- | --- | ---| 
| 20220405T12:13:41Z | Null | https://github.com/AtaturkUniversity-MSc/FuzzyLogic | 0 | 0| 
| 20220405T12:10:01Z | Succotash has reminded me of Sylvester from the Looney Tunes cartoons and his famous catch phrase %Sufferin succotash% ever since I heard of this one pot wonder. This simple dish originated in New England, USA prior to becoming popular in the southern United States and it was also a common meal in the Depression era. Succotash is essentially a meal of corn and lima beans although there are variations aplenty with additions such as tomatoes, capsicums/bell peppers, okra, other types of beans, butter, margarine, lard, bacon, fresh and dried herbs.  With some freshly harvested broad beans (also known as fava beans) from the garden begging to be used and corn and okra in the fridge I decided to make a version of succotash. I didn%t follow a particular recipe, instead my broad beans, corn, okra and tomatoes were plonked into a pot and stirred every so often. It had been a long day labouring in the garden and we were tired and hungry so I didn%t bother with double peeling the broad beans to save on time. Finely chopped basil and parsley along with margarine and seasonings were stirred through in the final minute before serving. | https://github.com/estelaboots/fuzzy-succotash | 0 | 0| 
| 20220405T12:00:40Z | MSc  | https://github.com/isakulaksiz/FuzzyLogic | 0 | 0| 
| 20220405T11:39:45Z | Imagine you could pick up a fragment of code in a complex system written in C and test it in separation on your Linux workstation without the burden of including all necessary headers and knowing the right set of #defines, compilation flags and the target architecture. Imagine you could use that code in a modern fuzzer or symbolic execution engine for thorough, focused deep testing.  AoT makes it possible to select a function from C code base and generate an executable off-target test harness. The harness can then be tested on a Linux machine, e.g. with ASAN, AFL or KLEE. The generated off-target is a self-contained binary and includes all the necessary types and definitions. In a nutshell, AoT makes it possible to test pieces of complex systems software in a unit test-like manner. What it is and how does this work?  First, you select a function F you are interested to test. AoT uses Code Aware Services (CAS) infrastructure, namely code database and compilation database to automatically pull in a subtree of functions called by F (that is, functions that F calls, functions that they call, etc.). By default, AoT stops at the module boundary: the functions compiled into the same module as F are pulled in, all the others are left out. For the functions that are left out AoT generates function stubs which can later be filled by the user. Such generated program is called an off-target, because it runs off the original code execution environment (e.g. a smartphone).  AoT works well with the AFL fuzzer (https://lcamtuf.coredump.cx/afl/) and the KLEE symbolic execution engine (http://klee.github.io/). It automatically generates binaries and test setup for those tools, so that you can start fuzzing the off-target immediately.  AoT is an automated solution that currently works in the human-in-the-loop model. It means that AoT tries to automate as much as possible, but a human operator is needed to fine-tune the results - e.g. provide stubs implementation or correct the program state initialization.  Potential uses of AoT are:      get a recursive list of functions given an entry point (could be used to get selective coverage)     get a list of types necessary for a given piece of code     instrument code for inter-structure fuzzing (unsupported yet)     instrument code for fuzzing / symbolic execution and apply those techiques to complex systems code     speed up development for slowly building targets (e.g. AOSP build process)  For example, let%s imagine we would like to test a message parser in a mobile phone modem. Normally, for such testing we need to set up the physical infrastructure, for example a base station that sends messages over the air to the mobile phone. When the message is received by the phone, the parser code is invoked. If there is an error, we need to collect potential crash logs (if any) and restart testing. The whole process is difficult to set up and a single testing cycle takes quite long. With AoT things look differently. We select the message parsing function as our target. AoT automatically pulls in the necessary definitions and functions compiled into the same module and generates function stubs for the functions outside of the module. Moreover, AoT generates the program state initialization and the code necessary for starting security fuzzing. The generated off-target code is self contained - we can compile it on a Linux box and use all standard tools such as fuzzers, gdb, sanitizers to test the code. As a result, we end up with a much faster setup and test cycle: the off-target generation takes minutes and we can re-execute the code up to thousands of times per minute. We can also easily attach a debugger and quickly inspect what went wrong.  As a further example let%s take the last point and let%s imagine we are modifying an AOSP kernel driver. Without AoT, we need to invoke entire build process to check if our change is correct. Moreover, we would need to run the code in an Android emulator or on the phone and find a way to invoke the changed driver code (which sometimes is not trivial). With AoT we can extract the code of the changed function and compile it within minutes. We can further use all available x86_64 Linux toolchains (gdb, sanitizers, etc.) to test it. As a result, the development & testing cycle should be much shorter. | https://github.com/Samsung/auto_off_target | 1 | 0| 
| 20220405T11:19:13Z | Null | https://github.com/movhiwwwc/fuzzy-disco | 0 | 0| 
| 20220405T11:04:57Z | Classify data in ms sql server using fuzzy wuzzy. | https://github.com/yonadav-labs/fuzzy-data-classifier | 0 | 0| 
| 20220405T11:02:56Z | Null | https://github.com/RiswanBasha/ComVeh-Fuzz-Testing-Tool | 0 | 0| 
| 20220405T09:59:05Z | Null | https://github.com/dflehel/fuzzyuni | 0 | 0| 
| 20220405T09:49:01Z | Null | https://github.com/nonamesec/restler-fuzzer | 0 | 0| 
| 20220405T09:36:35Z | Null | https://github.com/SHIVANI0708/Fuzzy-College | 0 | 0| 



# 日更新程序
