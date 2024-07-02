Java反射机制是指在运行时动态地获取和操作类的信息的能力。通过反射，我们可以在程序运行期间动态地分析、修改和调用类的方法、构造函数和字段等。这使得我们可以在不直接访问源代码的情况下，对类进行操作和扩展。
动态加载类：通过反射，我们可以在运行时根据需要动态加载类，而不需要在编译期间就将所有类都引入到项目中。这样可以节省内存空间，并且允许我们在运行时根据条件来选择加载不同的类。
动态创建对象：通过反射，我们可以在运行时根据类的信息动态地创建对象，而不需要在编译期间就知道具体的类名。这使得我们可以根据配置文件、用户输入或其他条件来创建不同的对象。
动态调用方法：通过反射，我们可以在运行时根据方法名和参数类型来动态地调用类的方法，而不需要在编译期间就知道具体的方法名和参数类型。这使得我们可以在不修改源代码的情况下，对方法进行扩展和调用。

Threadlocal：

调取清理方法，
把threadlocal定义为 private static

动态代理：
Jdk:通过接口实现,自己编写字节码文件。调取本类中的 方法会 不生效
Proxy.newproxyInstance -> $proxy.class -> sselect() -> Invocationhandler.invoke
Cglib:通过继承实现，ASM生成的字节码文件。调取本类中的 方法会 生效
Enhancer.create() -（ASM）>CGLB.class -> select() -> MethodInterceptor.intercept ->直接调用实现了被代理类的之类（动态代理类）到ASM

Autowired 和 Resource

HTTP协议：
状态码：

Mybatis
一级缓存：一级缓存是SqlSession级别的缓存。在操作数据库时需要构造sqlSession对象，在对象中有一个数据结构（HashMap）用于存储缓存数据。不同的sqlSession之间的缓存数据区域（HashMap）是互相不影响的。 一级缓存是默认开启的不用配置。
二级缓存：二级缓存是mapper级别的缓存，多个SqlSession去操作同一个Mapper的sql语句，多个SqlSession可以共用二级缓存，二级缓存是跨SqlSession的。二级缓存的开启（实体类必须序列化），然后在配置文件里面配置。


设计模式


锁

线程
创建 等待 运行 消亡 阻塞 


RUNNING  shutdown stop 
