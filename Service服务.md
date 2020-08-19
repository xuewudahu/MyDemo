### Service服务

1.service服务有两种方式启动 startservice() 和bindService()

startservice()与服务没有绑定，activity销毁后，sevice还会继续运行，没有联系了，想要service销毁可以通过activity中的stopService()或者是service中的stopSelf()方法。



bindservice()方法与服务器绑定，activity销毁后，service就销毁了，当在横竖屏转换时activity改变，service也会断开。绑定后启动onbind（）方法，销毁时启动onunbind()方法，任务是在onbind()方法返回的值。通过继承binder（内部实现了Ibinder接口），在通过实例化对象来创建供onbind()方法返回。

