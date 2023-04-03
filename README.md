# MobaXterm-GenKey
你懂的！！

## 本地启动
需要安装Python3!!!
```
pip install --no-cache-dir -r requirements.txt
python app.py
```

## Docker
```
docker pull malaohu/mobaxterm-genkey
docker run -d -p 5000:5000 malaohu/mobaxterm-genkey
```


## 使用方法
访问：IP:5000
![image](https://user-images.githubusercontent.com/8140841/116803404-e94c8300-ab49-11eb-83db-ad0246ebedd3.png)

### 激活方式
直接放到软件目录即可！
Flask版本要改下，不然运行会报错cannot import name 'escape' from 'jinja2'
Jinja 是 Fl​​ask 的依赖项，Flask V1.XX 使用escapeJinja 的模块，但是最近在新版本的 Jinjaescape中删除了对该模块的支持。

要解决此问题，只需在您的requirements.txt中更新到更新版本的 Flask V2.XX，其中 Flask 不再使用escape来自 Jinja 的模块。
原帖

requirements.txt内容改为Flask==2.1.0
解决


核心内容来自：https://github.com/flygon2018/MobaXterm-keygen
