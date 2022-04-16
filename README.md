# Custom-dependency-library-manual

# 1.首先为创建aar做准备  
修改aar项目里面的build Plugins,将application改成library  
![1650100577(1)](https://user-images.githubusercontent.com/84059192/163669578-13d42954-abde-4ffc-bf08-fa16edb30dc6.png)
# 2.准备制作maven库
## 1.创建新的gradle文件放在与aar的build同级目录下  
![1650100577(1)](https://user-images.githubusercontent.com/84059192/163669791-85e0ce04-5571-4db0-a57a-836db900b990.png)  
1.编写里面内容如下：  
![1650101535(1)](https://user-images.githubusercontent.com/84059192/163669890-f93dd15a-6058-4472-9e6e-47324f07eb7f.png)
2.编译通过后，点击Tasks-->Publishing-->publish  

