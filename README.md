# Simple-DNS-Server-with-learning
A Simple DNS Server with learning. Implemented DNS protocol.

使用程序流程：
1、配置数据库；使用MySQL导入该文件夹内dns.sql（范例数据库，内含一些常见网站）即可。
2、将config.txt中的default_dns=后的IP地址改为您的本地DNS服务器的地址。具体请WIN+R输入cmd，再输入ipconfig /all查看。
3、python环境已配置好。
4、修改dns配置.bat中的WLAN 2变成自己的网络连接名。用管理员权限运行dns_config.bat，将dns服务器地址改成本地回环。
5、在命令提示符中输入python main.py运行脚本；还支持一些参数，比如：
使用命令python main.py -h查看帮助。
-d为简单调试信息输出，-dd为复杂调试信息输出，二者互斥。
-s [本地DNS服务器地址]指定本地DNS服务器。
-f [配置文件路径]指定配置文件。
包含是否学习和默认本地DNS服务器地址（learning=1表示学习，0表示不学习）。
6、运行完后应运行dns_deconfig.bat改回原来的DNS配置。这个bat文件中也要将WLAN 2改成自己的网络连接名。

Attention：
dns_config.bat dns_deconfig.bat只支持Windows，Linux等其他系统下请自行配置

Contact：discat@foxmail.com
