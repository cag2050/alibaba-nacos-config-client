### Nacos 配置中心

### 注意：
1.本项目版本：

Spring Cloud Version| Spring Cloud Alibaba Version | Spring Boot Version
--- | --- | ---
Spring Cloud Greenwich | 2.1.1.RELEASE | 2.1.X.RELEASE

2.不要忘记在 Controller 类上加注解：@RefreshScope，主要用来让这个类下的配置内容支持动态刷新，也就是当我们的应用启动之后，修改了Nacos中的配置内容之后，这里也会马上生效；如果不配置该注解，修改了Nacos
中的配置内容之后，这里不会马上生效，重启本应用后再次读取才能看到修改的配置。

### 参考资料

参考资料 | 网址
--- | ---
Spring Cloud Alibaba基础教程：使用Nacos作为配置中心 | http://blog.didispace.com/spring-cloud-alibaba-3/
使用 Nacos 的 Docker 镜像，启动 Nacos 服务 | https://www.cnblogs.com/cag2050/p/11918293.html
组件版本关系 | https://github.com/alibaba/spring-cloud-alibaba/wiki/%E7%89%88%E6%9C%AC%E8%AF%B4%E6%98%8E