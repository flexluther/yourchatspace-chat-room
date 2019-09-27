# chat-room
Live Websocket Chat Room

chat room

Websocket chat room which supports tens of thousand of people online in a live chat environment. Realtime web chat system (client & server) based on websockets.

Stickers are placed in subfolders and loaded in tabs.
Minor interface changes, new default stickers and new sticker sets to download.
A new easy option to create your own notification file with 25 sounds to choose from.

yum install policycoreutils-python
semanage permissive -a httpd_t

You need an Apache module called proxy_wstunnel. You can enable proxy_wstunnel from a frontend such as cPanel, or:

Open /etc/httpd/conf.modules.d/00-proxy.conf and look for:

LoadModule proxy_wstunnel_module modules/mod_proxy_wstunnel.so

If not found, add the line at the end of the file and save.

Add to the config file of Apache (/etc/httpd/conf/httpd.conf) outside VirtualHosts:

ProxyPass "/MyWsServer/" "ws://localhost:9001/"

Save, restart Apache: systemctl restart httpd

For more information and demo link see chat room https://achatroom.co.uk


