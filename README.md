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
  
- 2020.10.24:

  - [ ] ByteCtf 尝试做了qiao 和 gun，qiao涉及了ollvm混淆就没做出来，gun的洞在哪也没找到

- 2020.10.25：

  - [x] qemu看完i440fx初始化，准备加速看一下那本书，理一下虚拟机初始化的过程，然后仔细看看源码
  - [x] 在wh1te师傅的帮助下，解出qiao，完成byetctf签到，ORZ
  - [ ] 整理qiao和easyheap的漏洞模式，但是没看出哪里有洞，ORZ

</details>

<details>
<summary>第十八周  ( 2020.10.26 - 2020.11.1 )  :  Qemu(六)</summary>

- 2020.10.26  :
  - [x] qemu 书看到fw_cfg设备那里，又回头看了下前面关于QOM那里的内容，对于qemu中实现的面向对象脑中有一个大概的框架，关于主板初始化，书中主板初始化这章也涉及了很多后面的章节的内容，不过对于主板初始化来说主要就是这几个步骤，创建北桥、创建PCI根总线、创建根PCI总线上北桥部分、创建初始化相关的MemoryRegion、创建PIIX3设备，对于虚拟机初始化来说，主要是下面几个步骤，内存计算，CPU初始化，内存初始化，主板初始化，中断初始化
  - [x] 分析了一下主板初始化的源码，不过没有分析完，复习了一下QOM相关的代码
  - [x] 两道leetcode题，第一道是计算数组中比当前数字小的数字的个数(利用二叉树思想做的)，第二道是判断是不是平衡树，方法是用前序遍历，每一次遍历都计算一次深度，然后做差进行对比
- 2020.10.27：
  - [x] qemu 书看完fw_cfg设备，fw_cfg设备主要的作用是用来给虚拟机转递信息的，包括给bios传递之前初始化过的主板上的硬件当中的信息，并且也可以给虚拟系统传文件，也可以起到像是一个微型的vmtools的作用。seabios并没有深究，因为这个seabios设计到的是bios的代码，和虚拟化感觉有关系但是关系并不是特别大，所以略读了一下
  - [x] 安好了codeql，简单的学了一些ql语法，审了一下freetype
  - [x] 两道leetcode题，第一道是二叉树的前序遍历直接套模板就可以了，第二道是求二叉树的最大深度这道题也是利用前序遍历，然后根据depth = max(depth(root->left) + depth(root->right)) + 1这个公式可以计算出来，左右子树的深度，然后找最大的就可以了
- 2020.10.28：

  - [x] 两道leetcode题，第一道是检测是不是对称的二叉树，第二道是把二叉树对称转换一下
- 2020.10.29：

  - [x] 社团招新，省赛备赛
- 2020.10.30：
  
  - [x] 社团招新，省赛备赛
- 2020.10.31：
  - [x] 社团招新，省赛备赛
  
- 2020.11.1：
  - [x] 社团招新，省赛备赛

</details>

<details>
<summary>第十九周  ( 2020.10.26 - 2020.11.1 )  :  虚拟化+备赛</summary>

-   2020.11.2：
  
  - [x] linux下的反调试，linux下的反调试的原理是因为gdb它动调的原理是使用ptrace，所以我们在程序里如果加了一句只可以被一个进程追踪的话，那么被gdb加载动调的时候就会直接结束
  - [x] 脱linux下的upx壳，脱upx壳就是利用ida远程动调，然后再利用idc脚本把程序dump出来，然后再进行之后的静态分析或动调调试
  - [x] 利用上面的两个知识点出了道题，攒fuzz机
  
-   2020.11.3：
    
    - [x] 尝试使用ptrace把反调试加固一下，加固的方法就是子进程所有执行的函数全部都是我们改写的函数，也就相当于一个小型的虚拟机，子进程中执行的是伪指令，真正的指令是在父进程中进行解释的，(准备用这个知识点出一道题)
    - [x] 复习一下base64加解密的原理
    - [x] 两道leetcode题，第一道是二叉树的最近公共祖先，最近公共祖先的定义为：“对于有根树 T 的两个结点 p、q，最近公共祖先表示为一个结点 x，满足 x 是 p、q 的祖先且 x 的深度尽可能大（一个节点也可以是它自己的祖先）这道题的解决方法是通过递归对二叉树进行后序遍历，当遇到节点 pp 或 qq 时返回。从底至顶回溯，当节点 p,q 在节点 root 的异侧时，节点 root 即为最近公共祖先，则向上返回 root；第二道是从上到下打印二叉树 II，这道题是使用的别人的方法，首先现根据当前结点，计算出下一层一共有多少个结点，然后打印本层结点的时候，每打印完一次，就把当前层结点数量减一，当节点数量为0时则打印完毕，当前层打印完毕就开始打印下一层
    
-   2020.11.4：

    - [x] 比赛备赛

    - [x] 两道leetcode题，第一道是寻找二叉搜索树中的第k大结点，二叉搜索树定义：二叉搜索树，它或者是一棵空树，或者是具有下列性质的二叉树：若它的左子树不空，则左子树上所有结点的值均小于它的根结点的值；若它的右子树不空，则右子树上所有结点的值均大于它的根结点的值；它的左、右子树也分别为二叉搜索树。利用的方法是二叉搜索树的中序遍历(左中右)为一个递增的有序序列，反中序遍历(右中左)为递减的有序序列，我起初的想法是遍历树上的所有结点，然后把所有的值存起来，然后对所有的值排序，排序之后再求第k大的结点，中间步骤太多所以超时了；第二道是二叉搜索树的最近公共祖先，和昨天做的那道二叉树的最近公共祖先一样的解法

      

