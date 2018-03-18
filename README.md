# spring-boot-starter-mongodb-plus

对官方spring boot starter对mongodb支持的扩展，提供更多配置属性，比如：连接数的配置等

## 如何使用

1. 在使用了`spring-boot-starter-data-mongodb`的项目中，增加以下依赖

```xml

```

2. 在应用主类上增加`@EnableMongoPlus`注解，比如：

```java
@EnableMongoPlus
@SpringBootApplication
public class Application {

    public static void main(String[] args) {
        SpringApplication.run(Application.class, args);
    }

}
```

## 配置参数

```properties

```
