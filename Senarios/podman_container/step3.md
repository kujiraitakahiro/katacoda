**Step3**  
コンテナイメージを取得します。  
podman images  
podman pull nginx  
podman images

取得したコンテナイメージからコンテナを起動します。  

podman ps(起動コンテナ一覧)  
podman ps -a(停止しているコンテナも含めて一覧表示)  

podman run --name nginx01 -d -p 8080:80 nginx  
```txt  
  --name：コンテナに任意の名前を付与  
  -d：バックグラウンドでコンテナを実施  
　-i：コンテナの標準入力を開く  
　-t：端末（TTY）を割り当てる  
　-p：公開ポートを指定（ポート変換）  
　  "-p 8080:80"とした場合、ホストOSのTCP8080番ポート経由で、コンテナのTCP80番ポートへアクセスする  
　--privileged：systemctlコマンドを使うための権限などを付与  
```

起動したら、確認しましょう。  
podman ps  
