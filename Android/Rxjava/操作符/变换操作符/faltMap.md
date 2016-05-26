# flatMap

将一个发射数据的Observable变换为多个Observables，然后将它们发射的数据合并后放进一个单独的Observable

FlatMap操作符使用一个指定的函数对原始Observable发射的每一项数据执行变换操作，这个函数返回一个本身也发射数据的Observable，然后FlatMap合并这些Observables发射的数据，最后将合并后的结果当做它自己的数据序列发射。

![](https://github.com/darkwh/MyNotes/blob/master/Android/Rxjava/resource/flatmap.png)

注意：如果任何一个通过这个flatMap操作产生的单独的Observable调用onError异常终止了，这个Observable自身会立即调用onError并终止。


- Javadoc: flatMap(Func1))
- Javadoc: flatMap(Func1,int))


# 个人理解
将一个(Observable)变为多个(Observable)，并将变换后的Observables的数据整合为一个单独的Observable.

flat；平坦，铺平     记忆方式：多个Observables整合为一个Observable，有铺平的意思，故为flatMap
