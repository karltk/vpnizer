Very rough shells scripts for setting up an OpenVPN server and generating client keys. 

 0. Build/buy/rent a server somewhere
 0. Make certain it's reachable on UDP port 1194
 0. `scp setup-vpn-server <public ip of your server>:`
 0. `ssh <public ip of your server>`
 0. `export SERVER_IP=<public ip of your server>`
 0. `sudo ./setup-vpn-server`
 0. An initial client config is available in `/etc/openvpn/easy-rsa/client`

For Android clients, a "fat" OVPN file is useful.

 0. `scp create-new-key <public ip of your server>:`
 0. `ssh <public ip of your server>`
 0. `sudo ./create-new-key phone`
 0. A "fat" OVPN file is available as `/etc/openvpn/easy-rsa/client/phone.ovpn`