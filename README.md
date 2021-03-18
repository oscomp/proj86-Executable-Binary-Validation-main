# proj-ELF-Validation

### 项目名称

在操作系统加载ELF文件时，校验ELF文件的合法性。

### 项目描述

一个功能完整的操作系统必须允许用户运行可执行软件（ELF或PE格式等），可执行文件可能还会依赖于某些动态链接库。但运行或引用未知来源或未经验证的可执行文件或动态链接库可能会破坏操作系统的安全机制，造成数据泄漏、系统崩溃或引发其它问题。

以通用Linux操作系统为例，Linux内核支持加载、运行静态或动态链接的ELF文件。可执行文件本身的加载必需由内核完成，而动态连接库的加载则既可以在内核中完成，也可通过解释器(ld-linux.so)在用户空间（glibc）完成。Linux内核和解释器都扮演了ELF文件加载器的角色，可以修改ELF文件加载器，在加载过程中校验可执行文件和动态链接库的合法性和完整性。

请设计并使用代码实现一套完整的流程，确保每个ELF文件（包括可执行文件和共享库）的可靠性和完整性。

### 所属赛道

2021全国大学生操作系统比赛的“OS功能设计”赛道

### 参赛要求

-   以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2021年春季学期或之后本科毕业的大一\~大四的学生）

-   如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖

-   请遵循“2021全国大学生操作系统比赛”的章程和技术方案要求

### 项目导师

-   金燕江

    -   github: jinyanjiang

    -   Email: jinyj@dingdaoos.com

-   张晓飞

    -   github: FelixZhang

    -   Email: zhangxf@dingdaoos.com

-   

### 难度

中等

### 特征

-   可实现对ELF文件的合法性校验

### 文档

无

### License

GPL v2

## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

-   基本目标：实现对ELF文件的合法性校验。需要同时提供流程描述和代码实现。

-   加分项：给出一套可行的验证方案，计算该实现对系统性能的影响。
