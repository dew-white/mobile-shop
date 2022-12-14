# 项目名称：白露在线-手机商城 介绍：MERN 全栈项目

## 用法

### ECMAScript Modules

项目的后端使用 ECMAScript 模块。确保至少具有 Node v14.6 +,
另外，在导入文件（不是包）时，请确保在末尾添加.js，否则会出现“找不到模块”错误

### 环境变量

在根目录中创建一个.env 文件，然后添加以下内容

NODE_ENV = development
PORT = 5000
MONGO_URI = 你自己的 mongodb uri /（应用测试使用：mongodb+srv://msonline123:msonline123@msonline.menjs.mongodb.net/mobileshop?retryWrites=true&w=majority）
JWT_SECRET = 'abc123'
PAYPAL_CLIENT_ID = 你的 paypal client id

### 安装依赖项（前端和后端）

```
npm install
cd frontend
npm install
```

### 运行 RUN

```
# 同时启动前后端 frontend (:3000) & backend (:5000)
npm run dev

#只启动后台
npm run server

```

### 打包与部署

```
# Create frontend prod build
cd frontend
npm run build
```

PS:有一个 heroku-postbuild 脚本，如果推送到 Heroku，则无需手动打包就可以部署

### 数据库测试数据

可以使用以下命令创建数据库测试用的用户和产品信息，以及销毁所有数据

```
# 插入数据
npm run data:import
# 销毁数据
npm run data:destroy
```

```
测试用户数据

admin@example.com (Admin)
123456

summer@example.com (Customer)
123456

henry@example.com (Customer)
123456
```
