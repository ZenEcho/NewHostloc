# NewHostloc新帖推送机
**为了多喝两碗汤**
原作者：https://github.com/w2r/hostloc2tg
# 使用说明

**1.到@BotFather创建一个机器人并保存Token值（若要推送到频道，将机器人添加到频道，并给予管理员权限）**

**2.获取chat id，方法忘了自己百度**

可以尝试一下是否可以发信息
```bash
https://api.telegram.org/bot这里填你的Token/sendMessage?chat_id=这里填频道id注意要加@&text=测试测试
```

# 服务器部署
```bash
git clone https://github.com/youheiss/hostloc2tg.git
yum install python3 
#安装requests，如果程序没运行起来多半是安装了Python2
pip3 install requests   
cd hostloc2tg 
#修改bot api token和chat id
vi hostloc2tg_api.py    
#最后运行：hostloc.txt是log出错了请自行排查
nohup python3 -u hostloc2tg_api.py >> hostloc.txt 2>&1 &
```


