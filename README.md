
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
