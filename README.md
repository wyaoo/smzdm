# 什么值得买 每日签到奖励 #
此脚本用于 [什么值得买](http://www.smzdm.com/) 网站的每日签到.

# 如何使用? #
脚本语言是`Python`, 所以首先你要[安装Python](https://www.python.org/downloads/)

然后脚本依赖于`requests`库, 所以你要[安装requests](http://www.python-requests.org/en/latest/user/install/)


```
vim ~/.bashrc
export SMZDM_DAILY_USERNAME='xxxxxxxx'
export SMZDM_DAILY_PASSWORD='xxxxxxxx'

crontab -e
0 6,18 * * * cd /root/gitsrc/smzdm && python smzdm_daily.py > /tmp/smzdm.log 2>&1
```


