# automatic_login_V2
锐捷校园网自动登录方案V2版

1.在v1的基础之上加入文件读取系统，能更好的应对加密密码随时间失效引发的登录失败
2.优化识别网卡机制
3.增加网络连通性测速以及优化win弹窗结构
4.发布版release 能直接运行，无需打包
5.兼容绝大部分windows系统版本的运行

使用技巧：
  #能自动登录锐捷校园网的方案

# 账号
#例如：2124281288
#""里面填写
userId=''

# 密码要加密后的，不能是加密前的
#例如：1f9fbf6d74588ac716f2090f8f372ab6667b699096b998baea6ea9801f2415ae3978e025d2d239b23af50a06a58040cc0bd219b46e7c1ba373676502edd22f2c3b240ad64ee3cf85facdfd8fa66b852778ff6453504dac1e6b0a22e9064f4104608f90135828ad95c9b4f0db265d6bd83ae7fbb9474c6a276d737538c92bda
#""里面填写
password=''

#多久入学填几几年
EPORTAL_USER_GROUP=''
#例：EPORTAL_USER_GROUP="2021"

# 如果不想执行输入自动登录就sc=多少就行（字符串类型）
#电信输入1，移动2，联通3，内网4
sc=''
#例：sc="2"

#dz是你们学校认证服务器的地址，不同学校地址不一样
dz='192.168.8.1'
# default 是校园内网
# ctc 是中国电信
# cmcc 是中国移动
# unicom 是中国联通
#自己办校园卡是什么运营商填什么，上面都给你了
EPORTAL_COOKIE_SERVER=''
#例如：EPORTAL_COOKIE_SERVER="cmcc"

#cookie 下面填需要你自己抓包，标头的cookie的最后有类似的，把JSESSIONID=""里面的内容复制粘贴就行
JSESSIONID=''
#例：JSESSIONID="093DD499BB09E5C421286D66CF430000"

#下一个版本会添加开机自启动脚本，不需要手动运行了
这个版本还是需要自己添加到计划任务里面

