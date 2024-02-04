# linux-command-for-DeepLearning
Record the basic linux command for DL 

## server use
连接服务器：ssh root@ip -p port  
查看服务器配置信息：neofetch  

## conda env
创建环境：conda create -n env_name python=3.9   
激活环境：source activate env_name   
退出环境：conda deactivate env_name     
删除环境：conda remove -n env_name --all     
克隆环境：conda create -n new_env_name --clone old_env_name    
重命名环境（只能先clone环境，再删除old name环境）   
列出所有环境：conda env list       
列出当前环境所有包：conda list     
导出环境配置：conda env export > environment.yml      
根据环境配置创建环境：conda env create -f environment.yml      

## GPU 
查看GPU资源： nvidia-smi  
查看nvidia显卡利用率，显存占用和算力情况：watch -n 0.5 nvidia-smi         #0.5秒更新一次显卡利用情况，并查看NVIDIA驱动版本  

## DeepLearning 
查看python端口：ps -ef |grep python  
中止进程：kill -9 pid  
后台运行命令：nohup python -u train.py &     
后台运行sh文件：nohup  ./run.sh &       
后台运行sh文件，并生成日志文件：nohup ./run.sh >log  2>&1 &

## file system
查看文件或者文件夹大小命令：du xxx(文件夹名称)         #注意，要在上层文件夹进行操作  
移除文件：rm  /-rf  filename  
复制文件夹：cp -r /a/ab/abc/* /m/mn/mnp/  
跨服务器传输文件：scp -P port -r transport_folder user@ip:/home/XXX/XXX/XXX  

