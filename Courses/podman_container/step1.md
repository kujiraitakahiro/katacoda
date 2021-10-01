**Step1**  
dockerパッケージがインストールされているか、確認します。  

rpm -qa | grep docker  
docker version  

※インストールされてますね。  


podmanと競合するため、dockerをアンインストールします。  

yum -y remove docker-ce*  
rpm -qa | grep docker  
