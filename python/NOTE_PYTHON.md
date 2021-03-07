# python笔记

python框架学习

## 数据读取

### dataset

+ dataset
  + 源码：多线程部分的源码应该是c编译的 TODO

+ *DataGenerator*

*dataset* 依赖 *DataGenerator*

```
# 依赖模块
import paddle.fluid.incubate.data_generator as dg

# 模版方法
# run_from_stdin 主要用这个
# run_from_memory
```

代码技巧：采用模版方法模式。模版方法内抽离的多态函数，全部返回一个 *iterator*(*tuple*类型)，从而实现了对这些接口的抽象。