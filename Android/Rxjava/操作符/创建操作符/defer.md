# defer

直到有观察者订阅时才创建Observable，并为每个观察者提供一个新的Observable（创建方式使用Observable工厂方法）

defer操作符接受一个你选择的Observable工厂函数作为单个参数

- javadoc:defer(Func0)

