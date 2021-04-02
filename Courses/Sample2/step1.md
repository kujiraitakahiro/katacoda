**Step1**  
nginx mainlineをインストールするために、  
レポジトリファイルを作成します。  

レポジトリファイル名：/etc/yum.repos.d/nginx.repo

nginx.reposの内容  
```txt
[nginx-mainline]
name=nginx mainline repo
baseurl=http://nginx.org/packages/mainline/centos/$releasever/$basearch/
gpgcheck=0
enabled=1
gpgkey=https://nginx.org/keys/nginx_signing.key
module_hotfixes=true
```
