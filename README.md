# webservice_server_demo
### webservice服务端创建
##### idea初始化创建webservice
> New -> Project... -> Java -> Web Application 勾选 WebServices -> Version 勾选 Apache Axis -> 点击 Next 生成项目

> 重要的一点：生成项目后，点击 File -> Project Structure... -> Artifacts : Fix 自己的项目

##### idea配置Tomcat，部署运行
> 注意：访问路径，我配置的是
http://localhost:8080

> 所以我的所有接口查看的url为 http://localhost:8080/services

> 定义的服务器接口类：
```
package example;

public class Test {
    public String test(){
        System.out.println("get test request success!");
        return "this is a test result!";
    }
}
```
