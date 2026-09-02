# SpringBoot Demo

GitHub Actions + Docker 自动部署到阿里云服务器示例项目。

## 本地开发

```bash
mvn spring-boot:run
```

访问 http://localhost:8080

## 接口

- `GET /` - 欢迎信息
- `GET /health` - 健康检查
- `GET /actuator/health` - Spring Actuator 健康检查

## 部署

推送到 main 分支自动触发 GitHub Actions 流水线：
1. Maven 打包
2. 构建 Docker 镜像
3. SSH 到阿里云服务器部署

## 服务器访问

部署后访问：http://115.29.229.16:8081
