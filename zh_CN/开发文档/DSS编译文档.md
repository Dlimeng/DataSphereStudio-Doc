## 1.编译整体的DSS：

   从git获取项目代码后，使用maven打包项目安装包。  

   (1) 您可以在最顶层的pom.xml文件，修改Linkis、Java、Scala、Maven等软件的版本，以适配您公司的大数据环境，具体如下：

```xml
  <properties>
          <dss.version>1.0.0</dss.version>
          <linkis.version>1.0.2</linkis.version>
          <scala.version>2.11.12</scala.version>
          <jdk.compile.version>1.8</jdk.compile.version>
          <maven.version>3.3.3</maven.version>
  </properties>

```

   (2) **如果您是本地第一次使用，必须在最外层工程pom.xml所在目录先执行以下命令**：

```bash
    mvn -N  install
```

   (3) 在最外层工程pom.xml所在目录执行以下命令
    
```bash
    mvn clean install
```

  

  (4) 获取安装包，在工程的assembly->target目录下：

```
    wedatasphere-dss-x.x.x-dist.tar.gz
```





