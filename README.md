# Wifi_share_on_ethernet_using_pi
We can share Raspberry pi wifi on ethernet port using script

We can execute ./wifi-to-eth-route.sh

for limit the internet speed use following command

sudo iptables -t nat -A POSTROUTING -o wlan0 -j MASQUERADE

sudo wondershaper wlan0 1000 1000     //uploading and downloading speed limit to 1000 kbps

sudo wondershaper clear wlan0        //clear internet speed limit
