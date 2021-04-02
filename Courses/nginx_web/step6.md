**Step6(参考)**  
この環境では"firewalld"は動作していませんが、  
起動してHTTPで使われるTPC80番ポートを解放します。  

systemctl start firewalld  
firewall-cmd --add-port 80/tcp --permanent  
systemctl reload firewalld  
firewall-cmd --list-all  


その後、再びWebサーバ(nginx)へアクセスします。  

上部にある"+"、"View HTTP port 80 on HOST 1"を順にクリックします。
