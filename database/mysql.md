# MySQL
---
[centos7 mysql数据库安装和配置](https://www.cnblogs.com/starof/p/4680083.html)

---
## 安装
## 首次登陆配置
1. 首次登陆
`mysql -u root `
- 设置密码安全等级
`SHOW VARIABLES LIKE 'validate_password%';`
`set global validate_password_policy=LOW;`
- 设置密码
`set password for 'root'@'localhost' =password('password');`
- 给root用户远程调试权限

- 配置端口转发