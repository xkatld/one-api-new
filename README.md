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

# Claude
激活 IAM Service Account Credentials API

https://console.cloud.google.com/apis/library/iamcredentials.googleapis.com?project=chat-408106

创建 application-default-credentials

https://cloud.google.com/docs/authentication/application-default-credentials

创建 application-default-credentials 的几个步骤

在 Service Account 页面新建 Service Account

在选择 Role 的时候需要选择 Vertex AI User (使用 Vertex AI 的权限) 和 Service Account Token Creater （生成 Access Token 的权限，用于 REST API 请求）

新建一个 Key

需要激活 IAM Service Account Credentials API
