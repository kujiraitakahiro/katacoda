**Step7(参考)**  
この環境では"firewalld"は動作していませんが、  
起動してsquidで使われるTPC8080番ポートを解放します。  

systemctl start firewalld  
firewall-cmd --add-port 8080/tcp --permanent  
systemctl reload firewalld  
firewall-cmd --list-all  
