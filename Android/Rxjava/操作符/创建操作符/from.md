# from 

将其它种类的对象和数据类型转换为Observable

from操作符可以转换Future、Iterable和数组

- Iterable和数组：
      产生的Observable会发射Iterable或数组的每一项

    示例代码：
    ```java
    Integer[] items = { 0, 1, 2, 3, 4, 5 };
Observable myObservable = Observable.from(items);

myObservable.subscribe(
    new Action1<Integer>() {
        @Override
        public void call(Integer item) {
            System.out.println(item);
        }
    },
    new Action1<Throwable>() {
        @Override
        public void call(Throwable error) {
            System.out.println("Error encountered: " + error.getMessage());
        }
    },
    new Action0() {
        @Override
        public void call() {
            System.out.println("Sequence complete");
        }
    }
);
```

- Future：发射Future.get()方法返回的单个数据

  - Javadoc: from(array))
  - Javadoc: from(Iterable))
  - Javadoc: from(Future))
  - Javadoc: from(Future,Scheduler))
  - Javadoc: from(Future,timeout, timeUnit))


