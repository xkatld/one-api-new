这是根据原项目最新修改编译，可能不稳定按需使用。
# 目前版本 v0.6.8-alpha.6
# 确保环境正确
环境：Debian12
```shell
apt update -y
apt install wget unzip git -y
git clone https://github.com/xkatld/one-api-new.git
cd one-api-new
unzip one-api.zip
chmod 777 one-api
./one-api --port 3000 --log-dir ./logs
```
# 注意事项
3000是端口 可以修改，默认账号密码也是root和123456，记得修改
