# camunda-spring-demo-boilerplate



Use https://start.spring.io/ to create your basic Springboot application.

![image-20240411155350104](/Users/william.marcq/Library/Application Support/typora-user-images/image-20240411155350104.png)





Add that code to pom.xml, get the version in https://mvnrepository.com/artifact/io.camunda.connector/spring-boot-starter-camunda-connectors

```xml
<dependency>
    <groupId>io.camunda.connector</groupId>
    <artifactId>spring-boot-starter-camunda-connectors</artifactId>
    <version>${version.connectors}</version>
</dependency>
```



Create your API credential

Console > Clusters (menu du haut)

Select cluster > API > Create new client

Give a name and select the scope (I recommend to check all) > Create

Copy to clipboard 

Add it to src/resources/application.properties

Open the terminal and try mvn spring-boot:run



If you have this kind of error no worries, it's not a blocking error, this is because you have an inbound  connector or webhook deployed on your cluster.

![image-20240411160933030](/Users/william.marcq/Library/Application Support/typora-user-images/image-20240411160933030.png)

If your terminal is waiting, it's OK.