# Linux多线程服务端编程

## 析构安全
1. [C++ shared_ptr线程安全问题]( http://www.boost.org/doc/libs/release/libs/smart_ptr/shared_ptr.htm#ThreadSafety
)
2. 使用`shared_ptr`时为什么指向的对象的头文件访问成员变量的函数不能内联?
3. 静态成员变量和类的关系?
4. [范型编程和面向对象的结合](http://www.artima.com/cppsource/top_cpp_aha_moments.html
)
5. 需要注意避免循环引用,通常的做法是 owner 持有指向 child 的 shared_ptr,child 持有指向 owner 的 weak_ptr。
6. 弱回调技术
7. enable_shared_from_this，[以派生类为模板类型实参的基类模板]( http://en.wikipedia.org/wiki/Curiously_recurring_template_pattern)
8. [孟岩的博客](http://blog.csdn.net/myan)
9. [shared_ptr](http://www.boost.org/doc/libs/release/libs/smart_ptr/shared_ptr.htm)

10. C++向前申明
11. eventfd vs pipe 唤醒方法

12. RAII handle 
13. Boost.Asio, Java Netty, Python Twisted
14. 各种处理模型以及对应的著名应用
15. gcc编译优化
16. [以小见大——那些基于 Protobuf 的五花八门的 RPC(2)](http://blog.csdn.net/lanphaday/archive/2011/04/11/6316099.aspx)
17. http://bulk.fefe.de/scalable-networking.pdf
    http://www.kegel.com/c10k.html
    http://gee.cs.oswego.edu/dl/cpjslides/nio.pdf
18. Accept惊群问题thundering herd
19. 使用非阻塞IO的注意事项（应用层Buffer）
20. 基于Reactor模式的开源网络库（libevent、muduo、Netty、twisted、POE）
使用**常引用**传递的规则，避免对象被反复拷贝。
