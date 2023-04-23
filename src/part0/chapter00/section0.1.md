> 作为开头，本节将带你解剖一只麻雀——你的计算机的组成。阅读完本节，你应当对计算机系统的研究内容有一个整体的印象。

# 0.1  从你的电脑讲起

计算机系统由两个个部分组成：

- 硬件
- 软件

## 硬件

计算机的硬件可以分为三大类：中央处理单元、主存储器和输入/输出子系统。

### 中央处理单元

在大多数体系结构中，CPU 有三个组成部分：

- 算术逻辑单元（ALU）：执行逻辑、位移和算术运算
- 控制单元：发送到其他子系统的信号，控制各个子系统的操作
- 寄存器组：存放零时数据的高速独立的存储单元

### 主存储器

主存储器是存储单元的集合。每个存储单元都有唯一的标识，称为**地址**。数据以称为**字**的位组的形式在内存中传入和传出。常见的字的大小为 32 位或 64 位。8 位称为 1 字节。

计算机用户需要很多存储器，尤其是速度快且价格低廉的存储器。然而存取速度快的存储器通常都不便宜，折中的办法是采用**存储器层次结构**：用较快的存储器存储经常访问的数据，用较慢的存储器存储不常访问的数据。

### 输入/输出子系统

I/O 子系统有如下分类，在此不做展开叙述：

- 非存储设备
    - 键盘和监视器
    - 打印机
- 存储设备
    - 磁介质：磁盘、磁带
    - 光存储：CD-ROM、DVD

### 子系统的互连

#### CPU 与存储器的连接

CPU 和存储器间通常由称为**总线**的三组线路连接在一起，分别是：数据总线、地址总线和控制总线。

#### I/O 设备的互连

输入/输出设备不能直接与总线相连，因为输入/输出设备的本质（机电、磁、光学设备）与 CPU 和内存（电子设备）不同，而且速度要慢得多。它们通过**输入/输出控制器**连接到总线上。

SCSI、火线、USB 和 HDMI 等都是控制器，它们清除了 I/O 设备与 CPU 和内存本质上的障碍。

- 串行控制器：只有一根数据线连接到设备上
- 并行控制器：有数根数据线连接到设备商，一次能同时传输多个位

## 软件

计算机软件分为两大类：操作系统和应用程序。计算机系统的研究对象是操作系统。

### 什么是操作系统

操作系统是计算机硬件和用户之间的接口，它使得其他程序能更加方便有效地运行，并能方便地对计算机硬件和软件资源进行访问。

### 操作系统概述

现代操作系统至少具有4种功能：

- 内存管理
- 进程管理
- 设备管理
- 文件管理

此外，还具有一个用户界面（或命令解释程序），负责系统与外界的通信。

### 主流操作系统

计算机用户熟悉的操作系统有三种：UNIX、Linux 和 Windows。

- UNIX 和 Linux 类似。它们是多用户、多进程、可移植的操作系统。UNIX 由四部分构成：内核、命令解释器、一组标准工具和应用程序。Linux 由三部分构成：内核、系统工具和系统库。
- Windows 是面向对象的、多层的操作系统，包括硬件抽象层、执行层和环境子系统层。