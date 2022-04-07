# NewHostloc新帖推送机

**为了多喝两碗汤**

原作者：https://github.com/w2r/hostloc2tg

# 使用说明

**1.到@BotFather创建一个机器人并保存Token值（若要推送到频道，将机器人添加到频道，并给予管理员权限）**

**2.获取chat id，方法忘了自己百度**

可以尝试一下是否可以发信息
```bash
https://api.telegram.org/bot这里填Token值/sendMessage?parse_mode=HTML&chat_id=这里填频道id值&text=这里是内容
```

# 服务器部署
```bash
git clone https://github.com/youheiss/NewHostloc.git
yum install python3 
#安装requests，如果程序没运行起来多半是安装了Python2
pip3 install requests   
cd NewHostloc
#修改bot api token和chat id
vi hostloc.py    
#最后运行：hostloc.txt是log文件出错了请自行排查
nohup python3 -u hostloc.py >> hostloc.txt 2>&1 &
```
# 效果
![image](https://user-images.githubusercontent.com/56901101/162135550-1024f317-f7dc-420e-8163-7a76527bc269.png)


