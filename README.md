# FinalSpeed备用安装方法


方法一：把这个源打包下载，将finalspeed_server.zip和install_fs.sh上传到主机，放在同一目录

方法二：使用wget命令把相关文件下载到主机

`wget https://github.com/gjc9620/FinalSpeed_LOCAL_INSTALL/master/finalspeed_server.zip`


`wget https://github.com/gjc9620/FinalSpeed_LOCAL_INSTALL/master/master/install_fs.sh`

`chmod +x install_fs.sh`

`./install_fs.sh 2>&1 | tee install.log`


debian,ubuntu下如果执行脚本出错,请切换到dash,
切换方法: sudo dpkg-reconfigure dash 选no


安装完后查看日志
tail -f /fs/server.log


卸载：
`sh /fs/stop.sh ; rm -rf /fs`

启动
`sh /fs/start.sh`

停止
`sh /fs/start.sh`

重新启动
`sh /fs/restart.sh`

运行日志：
`tail -f /fs/server.log`

windows客户端请下载Windows_client_1.2.exe