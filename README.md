这是根据原项目最新修改编译，可能不稳定按需使用。
# 确保环境正确
环境：Debian12
```shell
apt update -y
apt install wget unzip git -y
git clone https://github.com/xkatld/one-api-new.git
unzip one-api.zip
chmod 777 one-api
./one-api --port 3000 --log-dir ./logs
```

