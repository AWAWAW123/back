如何打开期末大作业(详细流程)
============================  
## 一、用gitpod打开项目链接  
在链接(https://github.com/qi-mo-zuo-ye/back) 前添加 https://gitpod.io#, 即新链接(https://gitpod.io/#https://github.com/qi-mo-zuo-ye/back)  
出现如下界面:
![gitpod打开](https://note.youdao.com/yws/api/personal/file/WEB67244d4937d43e0f14134b92c74cf900?method=download&shareKey=e41d71aad8092a794e44f4b5ef8a4d95)

## 二、安装Flask  
在gitpod控制台输入:                 
pip install bootstrap-flask                         
如图所示             
![控制台](https://note.youdao.com/yws/api/personal/file/WEBffa48278e0dca15d46de66f97c00e8f0?method=download&shareKey=4ccb547de3c6708246cbd6cc533e7578)       
回车确定后,出现以下内容,则安装完成           
![安装完成](https://note.youdao.com/yws/api/personal/file/WEBa9c947d2a3e0a771d02ac742b04cc223?method=download&shareKey=5ae233f42ea84379c1f08f33b1094986)         
## 三、打开运行   
在控制台输入如下内容:   
$ export FLASK_APP=flaskr    
$ export FLASK_ENV=development    
$ flask run   
并确定,如图所示          
![运行](https://note.youdao.com/yws/api/personal/file/WEB2a400f7c0a295cf9f38ccdab893fdaa9?method=download&shareKey=ab8aa0f24f6aabf478a36a35959e8170) 
在控制台输入   
flask init-db           
如图          
![输入](https://note.youdao.com/yws/api/personal/file/WEB894d110ae5dc78ad4a6a8788b8f82b45?method=download&shareKey=285102c9c557de7e3c1b1c03f8b665cd)   
再次输入:  
flask run         
如图               
![结果](https://note.youdao.com/yws/api/personal/file/WEB8648be912d3fe08f9a239ed97b36d3cf?method=download&shareKey=d2c4edda18bf00503b31ce95a7859d29)      

在控制台 CTRL+鼠标左键点击 http://127.0.0.1:5000/  打开网页     
    
    
![网页](https://note.youdao.com/yws/api/personal/file/WEB9e18f787e988a2c7bf197eb85941459e?method=download&shareKey=38dac52d88149066a4c1cb9abffa36ad)
## 四、网页使用     
按按钮跳转至对应页面                  
注册页面:      
![注册](https://note.youdao.com/yws/api/personal/file/WEB94d5fddeccf2aa162e09f2a6b2b69f6f?method=download&shareKey=a59057dcf7d233890ab12f7d29d6f5e7)        
登录页面:             
![使用1](https://note.youdao.com/yws/api/personal/file/WEB02fee65ec7e15bc0732df6d7d3b4a1bc?method=download&shareKey=c2633f2c98a8c6d7432ee00d9bd5581b)    
## 五、错误处理   
在使用网页注册,登录过程中,若确定后出现下图所示错误,可退回到上级页面。用户注册,登录操作已完成,不受错误页面影响。                  
![错误处理](https://note.youdao.com/yws/api/personal/file/WEBc09a4c8bb72cd03c784fd5b2157addc7?method=download&shareKey=5c3201e18bba6a260823376469a71a16)         
原因分析：         
登录以及注册后无法正常跳转, 似乎是因为redirect(url_for('auth.login'))无法在gitpod中正常的解析出url, 会解析出http://localhost:5000/auth/login          
## 六、手机显示      
![显示2](https://note.youdao.com/yws/api/personal/file/WEBf62f2b69fd6fd0dc3ee4773bf52c2c8d?method=download&shareKey=0ae9320d50ea1030f84bbe74e37d58a7)     
![显示1](https://note.youdao.com/yws/api/personal/file/WEB8e8230c3fb4b493503d8dfe6b4fb4bfe?method=download&shareKey=4e2413e09a39c26fc53412904e92652f)          
