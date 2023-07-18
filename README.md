# linux-command-for-DeepLearning
Record the basic linux command for DL 

## server use
连接服务器：ssh root@ip -p port  
查看服务器配置信息：neofetch  

## conda env
激活环境：source activate env_name

## GPU 
查看GPU资源： nvidia-smi  
查看nvidia显卡利用率，显存占用和算力情况：watch -n 0.5 nvidia-smi      #0.5秒更新一次显卡利用情况，并查看NVIDIA驱动版本  

## DeepLearning 
查看python端口：ps -ef |grep python  
中止进程：kill -9 pid  
后台运行命令：nohup python -u train.py &
后台运行sh文件：nohup  ./run.sh &  

## file system
查看文件或者文件夹大小命令：du xxx(文件夹名称)         #注意，要在上层文件夹进行操作  
移除文件：rm  /-rf  filename  
复制文件夹：cp -r /a/ab/abc/* /m/mn/mnp/  
跨服务器传输文件：scp -P port -r transport_folder user@ip:/home/XXX/XXX/XXX  

