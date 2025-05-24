## 飞比智能交付系统后端


### 构建
```
docker build -t cr.freeb.vip/freeb/fshop:dev .
```


### 启动
-   3.4 工程下输入
    ``` 
    mvn clean install package '-Dmaven.test.skip=true'
    ```
-   3.5 启动项目
    ```
    java -jar yshop-server/target/yshop-server.jar --spring.config.location=file:./yshop-server/src/main/resources/
    ```