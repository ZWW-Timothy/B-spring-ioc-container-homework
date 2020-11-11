主观题

@Component已经可以支持声明一个bean了，为何还要再弄个@Bean出来？

答：

@Component与@Bean的目的都是注册bean并装配到Spring容器中。

@Component一般通过路径扫描自动侦测与装配，@Bean一般在标有注解的方法中定义产生bean的逻辑。

@Bean相比于@Component，自定义性更强，用途更灵活，可以实现一些@Component实现不了的自定义加载类。

在引用第三方库中的类装配到Spring容器时，只能通过@Bean实现。
