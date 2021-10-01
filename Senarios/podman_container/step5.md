**Step5**  
コンテナを停止します。  

podman ps(起動しているコンテナ一覧)  

podman stop nginx01(コンテナの停止)  

podman ps -a(停止したコンテナを含めた一覧)  


続いて、コンテナを削除します。  
podman rm nginx01  

コンテナが削除されました。  
podman ps -a  
