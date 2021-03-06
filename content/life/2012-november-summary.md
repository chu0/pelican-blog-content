Title: 2012十一月总结和下月计划
Date: 2013-12-01 11:06
Update: 2013-12-02 15:18
Tags: 总结, 计划
Status: draft

[1]: https://github.com/mawenbao/gofeed "my github repo of gofeed"

十一月份很快也过去了，工作一如既往的闲，大部分时间都是在自学。生活上也是一如既往的平淡，没有好事也没坏事。偶尔有那么几次，或是上下班挤公交的时候，或是早上提前醒来的时候，我会忍不住想，自己是否活的太简单了，人生里最重要的阶段，就这么平淡的活下去，当某一天即将离开的时候，我能对自己说这一辈子我不后悔吗？

## 十一月总结

翻了下工作笔记和todo列表，除了些零散的知识外，最大的进步就是初步掌握了golang，并完成了[gofeed][1]这个开源工程。开发gofeed一方面是基于日常需要，一方面是为了练习golang。gofeed代码不多，大概1500行左右，但是涵盖了golang里的很多基础知识和相当一部分常用的标准库。说实话，golang虽然还不够成熟，但是论开发效率比python不遑多让，速度却比python好多了，以后也要当作自己的主力语言来研究才好。

十一月里有很多todo未完成，主要是一些知识和已解决问题没有总结，下个月记得先把老的todo清理掉。

## 十二月计划

下个月也就是十二月份，主要完成下面几件事。计划1比较庞大，如果工作比较忙，一个月可能无法完成，优先实现标记为(1)的部分。

1. 使用c++实现各种服务器端的并发模式
    *  先实现reactor pattern(1)和half sync/half async pattern。
    *  考虑分别使用epoll(1)，libevent/libev实现。
        *  后期应考虑可移植性。
    *  着重关注内存的申请和管理(1)，错误处理和监控，性能统计三件事。
    *  通讯协议可使用protobuf(1)。
    *  可使用zeromq实现通讯，和不使用zeromq做性能比较。
    *  代码应简单易读(1)。
    *  充分的说明文档，使用doxegen(1)生成API文档。
    *  单元测试(1)，最后总结时应包括测试代码的具体覆盖率。
    *  完成后写blog总结，应包括实现时的诸多设计考量，简单的类图和关键逻辑的时序图，最关键的是各个模式的benchmarking结果比较。
2. 阅读如下书籍
    *  结束"Effective C++, 2nd"，完成简单的阅读总结。
    *  回顾"Computer networking, a top-down approach"，复习基础的网络知识。
3. 把生词本里的众多钉子户干掉。
4. 背诵10篇新概念英语(三)。
5. 重构host-backup。

