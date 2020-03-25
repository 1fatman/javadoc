# Spring

1. **什么是Spring？为什么要使用Spring？好处是什么？**

   Spring是一个容器，Spring是轻量级的，并且Spring为Java Web企业级开发开发提供了一整套的解决方案

   

2. **什么是Spring IOC 容器？优点什么？**

   Spring IOC 负责创建对象，管理对象（通过依赖注入（DI），装配对象，配置对象，并且管理这些对象的整个生命周期。)

   优点：降低代码量，它使应用容易测试，单元测试不再需要单例和JNDI查找机制。最小的代价和最小的侵入性使松散耦合得以实现。IOC容器支持加载服务时的饿汉式初始化和懒加载

   

3. **Bean的生命周期**：Bean实例化——>Bean属性注入——>初始化（执行一系列的初始化前置操作）——>初始化成功（被使用）——>销毁

   

4. Spring框架包括：**Spring AOP，Spring ORM，Spring Web，Spring Web MVC，Spring Dao，Spring Context，Spring Core**

   

5. Spring中Java bean的作用域

   Singleton：单例   prototype：多个实例  request：每次Http请求都会创建一个bean

   session：在一个Http Seession中，一个bean定义对应一个实例

   global-session：在一个全局Http Session中，一个bean定义对应一个实例

   注：缺省默认为singleton

   