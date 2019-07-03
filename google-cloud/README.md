关于google cloud的一点分享

1.google cloud funciton 

google cloud function 提供给我们界面上的部署, 上传(功能代码), 终端的部署

至于界面上的部署, 请按照google cloud的介绍页面

下面对于google cloud function 终端部署的详解

准备工作(nodejs)

官方文档链接:
https://cloud.google.com/functions/docs/quickstart#functions-deploy-command-node8

- Python
- Nodejs

克隆好代码之后, 如果直接运行
gcloud functions deploy helloGET --runtime nodejs8 --trigger-http
会有问题

这里需要我们继续配置
1.google cloud账号的授权
gcloud auth login
输入该命令, 会跳转google的授权页

2.也可以设置默认的账号, 由于本人需要公司和个人账号切换, 所以直接login
gcloud config set account ACCOUNT

3.设置project id, project id 可以在最上面的`select a project` 看到
选择一个project id
gcloud config set project PROJECT_ID

4.如果要切换不同的id, 可以先不用设置,在部署的时候加上 --project=projectId 来设置
gcloud functions deploy helloGET --runtime nodejs8 --trigger-http --project PROJECTID