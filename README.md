# 计算机系统——从小白学起

Hello，欢迎来到计算机系统——从小白学起！这是一本致力于从零基础开始学习计算机系统知识，贯通数字逻辑设计、计算机组成、计算机体系结构以及操作系统四门经典的计算机系统课程的书，我们希望在这本书中实现以下与其他教科书不一样的特性：

1. 很多中文教科书对于初学者而言，文字描述晦涩难懂，更像是百科式的知识点罗列，细节描述也十分含糊，整体思路也不够清晰，本书希望做到语言描述清晰易懂，思路更加适合于初学者从零开始的接受能力，也更适合于构建完整的知识体系；
2. 国外教科书，特别是最经典的几本教材厚度足够劝退，并且其中语言描述有时略显冗余，全书通读性价比较低，并且其中许多重点或是细节的描述更像是一直在兜圈子，讲了很多，描述却仍旧十分含糊。本书希望在保证讲解清晰的同时语言精简，同时知识编排也更有条理；
3. 作为浙江大学信息安全系系统贯通课程的亲历者，笔者希望追随并扩展这一成功的试验，将四门计算机系统课程贯通，而非遵循传统的课程拆散，相互之间出现大量冗余内容的同时却仍然有许多内容都讲解不够深入的问题，从而构建完整的计算机系统知识与实验体系。

## 项目协作

非常欢迎大家参与到这一项目的构建中。由于作者精力与能力有限，很难高质量地完成本书的所有内容，因此非常需要更多对这一项目有热情的人参与进来。

## 项目构建

1. 安装 rust 工具链获取 cargo
2. 通过 cargo 安装 mdbook
    ```sh
    $ cargo install mdbook
    ```
3. 开启实时预览服务并在浏览器打开
    ```sh 
    $ mdbook serve --open
    ```
4. 构建
    - 本地构建
        ```sh 
        $ mdbook build
        ```
    - 远程部署：直接修改源码即可，GitHub Action 会针对每次 push 进行自动构建并部署到 GitHub Pages 上

## 项目规范

作为开源合作的中文计算机技术类书籍，本项目中写作规范应当遵守[中文技术文档写作风格指南](https://zh-style-guide.readthedocs.io/)，请在贡献前仔细阅读并核对格式。