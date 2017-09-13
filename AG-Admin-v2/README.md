# AG-Admin-v2
--------
# 项目结构
```
├─ace-security
│  │  
│  ├─ace-admin----------------管理端服务层
│  │  
│  ├─ace-gate-----------------网关负载中心
│  │ 
│  ├─ace-center---------------服务注册中心
│  │   
│  ├─ace-monitor--------------统一监控中心
│  │
│  ├─ace-config---------------统一配置中心
│  │
│  └─ace-api------------------公共服务接口包
│
```

# **AG-Admin启动指南**
# 启动指南
## 部署须知
- mysql数据库一个，redis数据库一个
- jdk1.8
- IDE插件一个，lombok插件，具体百度即可

## 运行步骤
- 运行数据库脚本：依次运行数据库：ace-admin/db/init.sql
- 修改配置数据库配置：ace-admin/src/main/resources/application.yml、ace-gate/src/main/resources/application.yml
- 依次运行main类：CenterBootstrap（ace-center）、ConfigServerBootstrap（ace-config）、GateBootstrap（ace-gate）、AdminBootstrap（ace-admin）
