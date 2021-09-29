**Step2**  
コンテナからコンテナイメージを取得します。  
今回は、nginxのコンテナイメージを取得します。  

docker images(保有するコンテナイメージの一覧表示)  
docker pull nginx(コンテナイメージの取得)  
　※latestタグ(最新版)が取得される  

docker pull nginx:1.21.3  
　※バージョン(タグ)指定も可能  

取得出来たら、docker imagesで取得したコンテナイメージを確認しましょう。  
docker images  

コンテナイメージの詳細を確認しましょう。  
docker image history nginx  
