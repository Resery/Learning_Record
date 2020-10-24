# Learning_Record

<details>
<summary>第一周  ( 2020.6.29 - 2020.7.5 )  :  STL(一)</summary>


- 弄完STL vector
- 补C++
- 南大计算机基础

</details>

<details>
<summary>第二周  ( 2020.7.06 - 2020.7.12 )  :  STL(二)</summary>


- 弄完STL list tree
- csapp 看到 2.3.2

</details>

<details>
<summary>第三周  ( 2020.7.13 - 2020.7.19 )  :  CSAPP Lab(一)</summary>


- Data Lab
- Bomb Lab
- Attack Lab
- Cache Lab

</details>

<details>
<summary>第四周  ( 2020.7.20 - 2020.7.26 )  :  CSAPP Lab(二)</summary>


- Malloc Lab
- Shell Lab

</details>

<details>
<summary>第五周  ( 2020.7.27 - 2020.8.2 )  :  Ucore Lab(一)</summary>

- 看完csapp
- Ucore Lab1

</details>

<details>
<summary>第六周  ( 2020.8.3 - 2020.8.9 )  :  Ucore Lab(二)</summary>


- Ucore Lab2-6
- Ucore 扩展做到 Lab1

</details>

<details>
<summary>第七周  ( 2020.8.10 - 2020.8.16 )  :  Ucore Lab(三)</summary>


- Ucore Lab7
- Ucore 扩展做到 Lab5

</details>

<details>
<summary>第八周  ( 2020.8.17 - 2020.8.23 )  :  Ucore Lab(四)</summary>


- Ucore Lab8
- Ucore 扩展做到 Lab7
- 整理6个关于整数/浮点数的CVE漏洞

</details>

<details>
<summary>第九周  ( 2020.8.24 - 2020.8.30 )  :  Ucore Lab(五)</summary>


- Ucore Lab 8 扩展
- 复现DirtyCow
- Makefile
- Google CTF sprint

</details>

<details>
<summary>第十周  ( 2020.8.31 - 2020.9.6 )  :  Ucore Lab(六)</summary>


- Ucore Lab 8 扩展
- 复现DirtyCow
- Makefile
- Google CTF sprint

</details>

<details>
<summary>第十一周  ( 2020.9.7 - 2020.9.13 )  :  Unix and P4CTF</summary>


- P4CTF KVM
- Unix 第一章

</details>

<details>
<summary>第十二周  ( 2020.9.14 - 2020.9.20 )  :  Unix and PlaidCTF</summary>


- PlaidCTF sandybox
- Unix 第四章

</details>

<details>
<summary>第十三周  ( 2020.9.21 - 2020.9.27 )  :  Qemu(一)</summary>


- Blizzard CTF
- Qemu 2.3
- ELF解析器

</details>

<details>
<summary>第十四周  ( 2020.9.28 - 2020.10.4 )  :  Qemu(二)</summary>


- Rdb调试器
- Qemu 2.5

</details>

<details>
<summary>第十五周  ( 2020.10.05 - 2020.10.11 )  :  Qemu(三)</summary>


- Qemu 3
- HITB CTF
- C语言实现面向对象
- 搭建漏洞复现环境

</details>

<details>
<summary>第十六周  ( 2020.10.12 - 2020.10.18 )  :  Qemu(四)</summary>


- day1: 搭建漏洞复现环境
- day2: 搭建漏洞复现环境
- day3: 复现CVE-2015-5156 写完 poc 和 exp
- day4: 复现CVE-2015-7504 分析完漏洞成因和执行流程
- day5: 复现CVE-2015-7504 写完 poc 由于涉及一个crc校验所以exp没有写出来
- day6: GACTF babyqemu
- day7: N1CTF Kemu 尝试做了一下  没做出来

</details>

<details>
<summary>第十七周  ( 2020.10.19 - 2020.10.25 )  :  Qemu(五)</summary>

- 2020.10.19  :  

  - [ ] N1CTF Kemu 没做完

- 2020.10.20：

  - [x] 2019 Qwb Qwct 这道题和之前的比起来就是多了一个对输入的数据会进行一些操作

    **漏洞模式1：当存储数据的buffer被填充满的时候，使用strlen得到的结果可能会是比理想值大的，因为其会把buffer后面的内容的长度也算进去**

    **漏洞模式2：以数组的size作为下标的时候，会导致读取或写入的时候，读取或写入到数组后面的区间**

- 2020.10.21：

  - [x] C++ prime 看了一下 以前没有注意到的章节
  - [x] 刷了两道LeetCode的简单题，一道是检验输入的字符是否是长按产生的利用双指针方法，一道是利用两个栈来替代队列使用的方法是一个栈用来主要存储数据另一个栈来辅助存储和汉诺塔比较类似

- 2020.10.22：

  - [x] Pwnable 3 道题，由于gdb环境崩了，所以就只做了3道，第一道start是个很简单的栈溢出然后往栈上写shellcode，第二道也是往栈上写shellocde使用orw，第三道有趣一些是一个计算器不过计算器对数据处理的不够细致在输入如"+666"这种数据的时候会导致越界读或写
  
- 2020.10.23：

  - [x] N1CTF Kemu  收尾，以前没遇见过的题目类型，修改了原有的qemu设备代码，而不是自己新添加的设备，而且还涉及到了一个附属设备的东西