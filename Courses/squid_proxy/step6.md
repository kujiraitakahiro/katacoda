**Step6**  
Proxyの動作を確認します。

以下のような通信フローとなり、squidのログファイルを確認します。  
クライアント(curlコマンド) ⇔ Proxy(squid) ⇔ Webサイト  

curl https://www.opensourcetech.tokyo/  
cat /var/log/squid/access.log  
