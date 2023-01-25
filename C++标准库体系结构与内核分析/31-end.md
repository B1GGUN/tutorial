## 仿函数和函数对象
![[311.png]]

![[312.png]]
unary_function是一个操作数，例如一个数取负；
binary_function是两个操作数，例如两个数相加。

整体上没啥好记的。
***
## Adapters
![[321.png]]

adapters内含想内含的。如容器适配器就内含一个容器。

例如，容器适配器：
![[322.png]]

函数适配器：
![[331.png]]
bind2nd绑定第二个参数，

not1：一样。
![[341.png]]
整体意义就是    不（小于40的数）

没啥讲的。
***
## bind
![[332.png]]

![[351.png]]
bind能绑定：
1. functions
2. function objects
3. member functions, \_1必须是某个object的地址
4. data members, \_1必须是某个object的地址

\_1是placeholders占位符，例如(\_1, 20) == (x, 20)

```cpp
bind<int>(my_divide, _1, _2)  // 将返回类型转换为int

bind(&MyPair::multiply. _1) //绑member function时 内含一个this
```
***
## 迭代器适配器
![[361.png]]

![[371.png]]
重载"=",很牛逼。

![[381.png]]

ostream_iterator, istream_iterator略，不想看。
***
后面还有个第四章不想看了 感觉不重要 累了



https://blog.csdn.net/daaikuaichuan/article/details/80717222
https://www.cnblogs.com/xiaokang01/p/12460786.html
https://zhuanlan.zhihu.com/p/476016358



