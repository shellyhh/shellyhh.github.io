## 启动nginx命令：
1. sudo /etc/init.d/nginx start
* sudo /usr/bin/nginx -c config_file
* sudo service nginx start

## 关闭nginx命令:
1. sudo /etc/init.d/nginx stop
* sudo service nginx stop
* kill -QUIT $( cat /usr/local/nginx/logs/nginx.pid )
*  /usr/bin/nginx -s stop 

**tip:**
`nginx.pid 文件位置可以查看nginx.conf 里面具体配置`

| 信号值 | 说明 |
|-----------------|-----------------------|
| TERM, INT |	Quick shutdown |
|QUIT |	Graceful shutdown |
| KILL |	Halts a stubborn process |
| HUP |	Configuration reload  Start the new worker processes with a new configuration Gracefully shutdown the old worker processes |
| USR1 |	Reopen the log files |
| USR2 |	Upgrade Executable on the fly |
|WINCH |	Gracefully shutdown the worker processes |

未完待续。。。。。。
