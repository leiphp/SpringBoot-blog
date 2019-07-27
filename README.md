# SpringBoot-blog
SpringBoot+vuejs搭建个人博客

### 构建项目
1.图形化构建方式（http://start.spring.io/）  
2.命令行方式（Maven）  
`mvn archetype:generate -DinteractiveMode=false -DgroupId=cn.lxtkj -DartifactId=demoapp-maven -Dversion=1.0.0-SNAPSHOT`  
### 多模块项目 
1. 调整主（父）工程类型（packaging） 
2. 创建子模块工作（module）  
    * 模型层：model  
    * 持久层：persistence 
    * 表示层：web 
3. 子模块依赖管理（dependencyManagement）  
4. 项目打包方式 
   * 构建Jar包 
   * 构建war包
   * 构建ear包  
   打包命令:`mvn -Dmaven.test.skip -U clean package`  
   jar包启动方式：切换到target目录输入命令 `java -jar first-app-demo-0.0.1-SNAPSHOT.jar`  
5. 运行模式
   * IDEA方式
   * JAR/WAR方式  `java -jar first-app-demo-0.0.1-SNAPSHOT.jar`  
   * Maven插件方式  
     * 1.首先回到根目录 `F:\github-project\SpringBoot-blog` 
     * 2.输入命令：`mvn spring-boot:run`



