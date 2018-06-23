# weibo
一个自动每天发微博的脚本

之前大一的时候初学python为了练手写的一个小东西，一直在服务器上跑，没当回事。因为前两天发现博客登不上去才发现服务器宕机了，重启后想重新把这个脚本跑起来还要去源代码里面改执行日期，很是麻烦，于是这次把代码整理了一下添加了一些功能：

1、命令行选项

  -h, --help          show this help message and exit
  
  -t T, --time=T      -t 设定每天几点发。如 -t 8；默认4点发，24小时制。
  
  -p, --picture       -p 随机发送图片
  
  -y, --yingyingying  -y 报时+卖萌
  
  -r, --random        -r 每天从以上内容中随机选择一种发送
  
  例如 python SentWeiBo_Console.py -h 19 -p 就是每天19点发送一次图片
  
2、添加了随机发图片的功能，之前只有报时功能。只要把文件放到和脚本同一目录下的pic文件夹中即可

3、进程守护，这个东西本来是跑在搬瓦工上守护shadowsocket的，手动改一下即可

还想要添加的功能：

1、自定义内容，现有上述两个功能。

2、自定义发送频率

粗略的想了一下不太好弄，以后有机会再说吧
