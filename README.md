# get_wechat
# 微信个人信息爬取
# 一、检测是否被对方用户删除：
1、原理就是新建群组,如果加不进来就是被删好友了(不要在群组里讲话,别人是看不见的)
2、目前的问题是，新建群组，添加好友的接口存在数量限制。在一定时间内添加的总人数超过一定数量后，接口就会无法使用。
# 二、微信好友数据获取：
1、利用requests库，对微信端发起请求，生成二维码扫描授权登录，对好友列表的信息进行扫描下载个人信息和头像，并调用csv包将数据存为csv格式，进而储存为excel列表格式
2、可改进点：可以进一步对好友的特点进行统计，如：好友省份统计图，好友性别统计图等数据统计可视化分析（可以使用tybleau或利用python自带matplot库）
