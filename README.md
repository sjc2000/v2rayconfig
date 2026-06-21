前置工作：

  1.安装BBR

      wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh 
	  chmod +x bbr.sh
	  bash bbr.sh
      lsmod | grep bbr
  
  2.开放防火墙端口
  
      sudo firewall-cmd --permanent --add-port=13908/udp
      sudo firewall-cmd --permanent --add-port=30000-50000/udp
      sudo firewall-cmd --reload
  
  3.优化网络参数
  
      修改etc/sysctl.conf
      修改etc/security/limits.conf
  
      
