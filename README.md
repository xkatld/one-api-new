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

# Vertex Claude 
激活 [IAM Service Account Credentials API](https://console.cloud.google.com/apis/library/iamcredentials.googleapis.com?project=chat-408106)

创建 [application-default-credentials](https://console.cloud.google.com/projectselector2/iam-admin/serviceaccounts?supportedpurview=project)

在 Service Account 页面新建 Service Account

![image](https://github.com/user-attachments/assets/39eebca3-a94c-4959-86ab-902ced1a67e9)

在选择 Role 的时候需要选择 Vertex AI User  和 Service Account Token Creator

![image](https://github.com/user-attachments/assets/1623b07e-5344-4552-9d7b-5e2e509d0893)

生成下载JSON

![image](https://github.com/user-attachments/assets/c024084b-66e3-48e5-9c40-adb9a5cdc786)
