[toc]

学习计划：

JAVA--Kotlin基础--安卓基础--编写测试DEMO--项目--业务逻辑





## 项目说明

写写 Demo、练练代码是非常重要的实践过程，可以帮助你更好地掌握所学的知识。我们可以通过一个具体的示例来解释如何完成这些练习，比如：解析 JSON 数据并用 MVC 分层架构实现一个简单的列表展示页面。

### 实践示例：微信首页

我们将创建一个简单的微信首页，其中包括一个列表，数据从网络上的 JSON 数据获取并解析成模型，使用 MVC 架构来组织代码。

#### 准备工作

1. **创建项目**

   - 打开 Android Studio，创建一个新的项目，选择 Empty Activity 模板。
   - 为项目命名，例如 "WeChatHomeDemo"。

2. **添加依赖**

   - 在 

     ```
     build.gradle
     ```

      文件中添加以下依赖：

     ```
     gradle复制代码implementation 'com.squareup.retrofit2:retrofit:2.9.0'
     implementation 'com.squareup.retrofit2:converter-gson:2.9.0'
     implementation 'androidx.recyclerview:recyclerview:1.2.1'
     ```

#### 目录结构

```pascal
app/
├── java/
│   └── com.example.wechathomedemo/
│       ├── controller/
│       │   └── MainActivity.java
│       ├── model/
│       │   └── Contact.java
│       │   └── ApiService.java
│       ├── view/
│       │   └── ContactAdapter.java
│       └── network/
│           └── RetrofitClient.java
└── res/
    ├── layout/
    │   └── activity_main.xml
    │   └── item_contact.xml
    └── values/
        └── strings.xml
```