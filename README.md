# customizeSprintBootStarter

这个关键步骤就是：
1. 要创建META-INF\spring.factories:
   org.springframework.boot.autoconfigure.EnableAutoConfiguration=com.demo.starter.config.DemoConfig
2. DemoConfig里面用@Configuration @Bean

3.使用的时候再引入dependency就可以：
    <dependencies>
        <!-- 自定义starter -->
        <dependency>
            <groupId>com.shishi</groupId>
            <artifactId>shi-spring-boot-starter</artifactId>
            <version>1.0-SNAPSHOT</version>
        </dependency>
    </dependencies>

    
这样就有了自定义的bean注入到了容器中
