# repeat 

repeat重复地发射数据。某些实现允许你重复的发射某个数据序列，还有一些允许你限制重复的次数

repeat不是创建一个Observable，而是重复发射原始Observable的数据序列，这个序列或者是无限的，或者通过repeat(n)指定重复次数。

repeat操作符默认在trampoline调度器上执行。有一个变体可以通过可选参数指定Scheduler。

- Javadoc: repeat()) 
- Javadoc: repeat(long)) 
- Javadoc: repeat(Scheduler)) 
- Javadoc: repeat(long,Scheduler))
