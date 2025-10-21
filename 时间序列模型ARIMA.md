# 时间序列模型ARIMA

## 1. 模型介绍

要学习时间序列模型，首先我们要理解并区分**时期序列**和**时点序列**。
1. **时期序列**中的观测值反映现象在一段时期内发展过程的总量，不同时期的观测值**可以相加**，相加结果表明现象在更长一段时间内的活动总量，如中国过去10年的GDP序列；
2. **时点序列**中的观测值反映现象在某一瞬间上所达到的水平，不同时期的观测值**不能相加**，相加结果没有实际意义，如某地每隔一小时测得的温度数据。

```flow
st=>start: 开始框
op=>operation: 处理框
cond=>condition: 判断框(是或否?)
sub1=>subroutine: 子流程
io=>inputoutput: 输入输出框
e=>end: 结束框
st->op->cond
cond(yes)->io->e
cond(no)->sub1(right)->op
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTI5OTAxOTk5NSw0MjI4NDg1MDNdfQ==
-->