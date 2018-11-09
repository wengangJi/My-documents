 # Wayne
 
 Wayne是一个通用的、基于Web的Kubernetes多集群管理平台。允许用户同时运行和管理多个Kubernetes集群的应用，同时支持json和yaml两种模式编辑模版。并且具有完整的权限管理系统，适应多租户场景。
 Wayne是一个通用的、基于Web的Kubernetes多集群一站式可视化管理平台。内置了丰富多样的功能，满足企业的通用需求，同时插件化的方式可以方便集成定制化功能。
 
 ![Dashboard UI workloads page](docs/images/dashboard-ui.png)
 
 ## Features
 Wayne已大规模服务于360搜索，承载了公司绝大部分业务，稳定管理了上万个容器。
 
 - RBAC（Role based access control）：用户通过角色与部门和项目关联，拥有部门角色允许操作部门资源，拥有项目角色允许操作项目资源，更加适合多租户场景。
 ![Dashboard UI workloads page](docs/images/dashboard-ui.png)
 
 - Json/Yaml支持：同时支持Json和Yaml两种编辑模式。
 
 - LDAP/OAuth2/DB多种登录模式支持：集成企业级LDAP登录及数据库登录模式，同时还可以实现插件实现OAuth2登录。
 
 - 支持同时管理多集群：可以同时管理多个Kubernetes集群，更方便的多集群管理。
 ## Features
 
 - 完整审计：每次操作都会有完整的审计功能，追踪用于操作历史。
 - 可视化操作：提供直观、简便的方式操作Kubernetes集群，减小学习成本，快速上线业务。
 - 多样的编辑模式：支持图形化编辑，也支持Json、Yaml两种高级定制化编辑模式。
 - 微内核架构：采用可扩展的插件化方式开发，定制化选择特性功能，更方便的集成符合企业需求的新功能。
 - 多集群管理：可以同时管理多个Kubernetes集群，更方便的管理多个集群。
 - 丰富的权限管理：将资源抽象化为部门、项目级别，角色的权限可以更细化的控制，适用于多部门、多项目的统一集中管理。
 
 - 多种登录模式：支持企业级LDAP登录、支持OAuth2登录，支持数据库登录多种模式。
 - 完备的审计：所有操作都会有完整的审计功能，方便追踪操作历史。
 - 开放平台：支持APIKey开放平台，用户可自主申请相关APIKey并管理自己的项目。
 - 多层次监控：提供多级别的监控统计信息，实时关注集群的运行状态。
 
 
 - 基于Web图形界面：相对于命令行管理集群更加直观和简便。
 
 ## 架构图
 
 整体采用前后端分离的方案，其中前端采用Angular框架进行数据交互和展示，使用Ace编辑器进行Kubernetes资源模版编辑。后端采用Beego框架做数据接口处理，使用Client-go与Kubernetes进行交互，数据使用MySQL存储。
 整体采用前后端分离的方案实现。
 
 - 前端采用Angular框架进行数据交互和展示，使用Ace编辑器进行Kubernetes资源模版编辑。
 
 - 后端采用Beego框架做数据接口处理，持久层采用MySQL存储，使用client-go与Kubernetes进行交互。
 
 ![Dashboard UI workloads page](docs/images/architecture.png)
 
 
 
 ## 项目依赖
 
 - Golang 1.9+([installation manual](https://golang.org/dl/))
@@ -35,6 +44,8 @@ Wayne鏄竴涓氱敤鐨勩佸熀浜嶹eb鐨凨ubernetes澶氶泦缇ょ鐞嗗钩鍙般傚厑璁哥
 - MySQL 5.6+  (Wayne主要数据都存在Mysql中)
 - RabbitMQ (事件消息通道,例如审计日志)
 
 
 
 ## 文档
 
 Wayne文档包含以下四类文档：
@@ -49,6 +60,8 @@ Wayne鏂囨。鍖呭惈浠ヤ笅鍥涚被鏂囨。锛
 
 [完整文档链接](http://docs.qihoo.cloud)
 
 
 
 ## 项目规划
 
 - 国际化
@@ -58,8 +71,12 @@ Wayne鏂囨。鍖呭惈浠ヤ笅鍥涚被鏂囨。锛
 - 支持HPA等其他对象
 - 支持运维Kubernetes集群，提供Kubectl所有功能
 
 
 
 ## 贡献者
 
 内部开发过程中有些开发者未在Contributors中，在此一并列出[@wilhelmguo](https://github.com/wilhelmguo),[@codeb2cc](https://github.com/codeb2cc),[@chengyumeng](https://github.com/chengyumeng),[@BennieMeng](https://github.com/BennieMeng)
 
 ## License
 
 
 ## License
\ No newline at end of file
