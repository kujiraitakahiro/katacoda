**Step8**  
nginxを起動します。  
起動後、状態を確認します。  

systemctl start nginx  
systemctl status nginx  

また、SELinuxを無効化します。  
setenforce 0  
getenforce  
