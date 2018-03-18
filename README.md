# spring-boot-starter-mongodb-plus

对官方spring boot starter对mongodb支持的扩展，提供更多配置属性，比如：连接数的配置等

## 如何使用

1. 在使用了`spring-boot-starter-data-mongodb`的项目中，增加以下依赖

```xml
<dependency>
    <groupId>com.spring4all</groupId>
    <artifactId>mongodb-plus-spring-boot-starter</artifactId>
    <version>1.0.0.RELEASE</version>
</dependency>
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

可配置参数如下：

```properties
spring.data.mongodb.option.min-connection-per-host=0
spring.data.mongodb.option.max-connection-per-host=100
spring.data.mongodb.option.threads-allowed-to-block-for-connection-multiplier=5
spring.data.mongodb.option.server-selection-timeout=30000
spring.data.mongodb.option.max-wait-time=120000
spring.data.mongodb.option.max-connection-idle-time=0
spring.data.mongodb.option.max-connection-life-time=0
spring.data.mongodb.option.connect-timeout=10000
spring.data.mongodb.option.socket-timeout=0

spring.data.mongodb.option.socket-keep-alive=false
spring.data.mongodb.option.ssl-enabled=false
spring.data.mongodb.option.ssl-invalid-host-name-allowed=false
spring.data.mongodb.option.always-use-m-beans=false

spring.data.mongodb.option.heartbeat-socket-timeout=20000
spring.data.mongodb.option.heartbeat-connect-timeout=20000
spring.data.mongodb.option.min-heartbeat-frequency=500
spring.data.mongodb.option.heartbeat-frequency=10000
spring.data.mongodb.option.local-threshold=15
```

**上述配置值均为默认值**
