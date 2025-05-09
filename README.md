 <center>
     <h1>罗峰</h1>
 </center>

## 个人信息

* 性 别：男&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;年 龄：35
* 手 机：18250847065 &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;  邮 箱：lfeng1417@outlook.com
* 专 业：计算机科学与计算 &emsp;&emsp;&emsp;&emsp;&emsp; 岗 位：研发工程师

## 工作及教育经历

* 华为通信技术有限公司&emsp;&ensp;2019.8-至今&emsp;&emsp;&emsp;&emsp;&emsp; 2012部门、华为云&emsp;&emsp;研发
* 厦门大学&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;2014.9-2017.7&emsp;&emsp;&emsp;&emsp; 计算机技术专业&emsp;&emsp;&emsp;研究生

## 专业技能

* 熟练使用 C++、Go，了解 Java、Python等编程语言
* 掌握基础数据结构和算法的基本原理
* 掌握

## 项目经验
**项目背景**：针对华为自研鲲鹏芯片进行系统级和编译器级优化，提升应用性能。  
**优化方法**：  
- **系统调优**：  
  - 使用 `top`、`mpstat`、`free`、`iostat`、`sar` 等工具分析 CPU、内存、磁盘 I/O、网络等瓶颈。  
  - OS 调优：进程绑核、NUMA 优化、大页内存、透明大页、脏页比例调整、网卡中断绑核、`ulimit` 优化等。  
- **编译器优化**：  
  - 调整优化等级，使用 PGO、LTO、CSPGO、AutoFDO 等优化手段。  
  - 内存优化：鲲鹏指令矢量化（`wrap-memset/memcpy`）、数据预取、结构体指针压缩、`jemalloc` 优化。  
  - 代码优化：`restrict` 关键字减少别名分析开销、`#pragma unroll` 循环展开、近似计算优化（牛顿迭代法替代除法）。  
**优化案例**：  
1. **Nginx 性能劣化定位**  
   - OpenEuler 2203.SP2 相比 CentOS 性能劣化 150%+，通过 `strace` 发现 `newfstat` 系统调用导致额外开销。  
   - 回退 OpenEuler SP3 的 `glibc` 补丁后性能恢复，并优化网卡中断绑核策略。  

2. **GTS 计费应用编译优化**  
   - 毕昇编译器相比 GCC 10.3 性能劣化 18%，通过 `perf` 分析发现指令缓存缺失率增加 5%。  
   - 定位到 `-fno-plt` 选项在 AArch64 未生效，导致动态库调用额外 `plt` 函数，最终通过补丁修复性能问题。  

3. **语音合成软件性能调优**  
   - 分析 `perf` 热点发现内存访问瓶颈，通过鲲鹏预取指令优化矩阵计算函数，结合 `jemalloc` 和 PGO，性能提升 10%。  

## 获奖经历

* 
* 
* 

## 个人账号

* https://blog.csdn.net/helloeveryon?type=blog
* https://github.com/lfeng14?tab=repositories

## 其他信息

* 喜欢专研
* 
