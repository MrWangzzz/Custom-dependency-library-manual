# Custom-dependency-library-manual

# 1.首先为创建aar做准备  
修改aar项目里面的build Plugins,将application改成library  
![1650100577(1)](https://user-images.githubusercontent.com/84059192/163669578-13d42954-abde-4ffc-bf08-fa16edb30dc6.png)  
# 2.创建Gitee库
创建完后clone到本地
# 3.准备制作maven库
## 1.创建新的gradle文件放在与aar的build同级目录下  
![1650100577(1)](https://user-images.githubusercontent.com/84059192/163669791-85e0ce04-5571-4db0-a57a-836db900b990.png)  
### 1.编写里面内容如下：  
![1650101535(1)](https://user-images.githubusercontent.com/84059192/163669890-f93dd15a-6058-4472-9e6e-47324f07eb7f.png)  
mavenDirPath的地址换成刚刚clone下来的的库地址  
### 2.编译通过后，点击Tasks-->Publishing-->publish  
![1650101830(1)](https://user-images.githubusercontent.com/84059192/163670053-a64340f2-0660-4f66-8cc0-0d2dbf2ebf06.png)
### 3.将生成的文件上传gitee
# 4.如何使用
## 1.将库的url填入 maven  
![1650102376(1)](https://user-images.githubusercontent.com/84059192/163670338-a82460a8-f8f7-47e2-8844-368a55d7e76f.png)
## 2.引入依赖
![image](https://user-images.githubusercontent.com/84059192/163670374-86f23faa-fe78-40ca-b6ca-bbfdbd65ad81.png)
# 有可能出现的问题
## 1.Could not find com.android.tools.lint:lint-gradle:30.0.2.
在项目的根build.gradle中的全局repositories里面添加google()  
## 2.Could not find org.codehaus.groovy:groovy-all:3.0.7.
在项目的根build.gradle中的全局repositories里面添加jcenter()  
