# WindowsGSM.Repoly

🧩 A plugin version of the Repoly Dedicated server for WindowsGSM

## Notes
- its recommended to start with embedd console, else the Starting state will not go away
- for further config: Click on the server entry, then Browse => ServerFiles check the file RePoly/Saved/Config/WindowsServer/Game.ini 
	- see screenshot of the Documentation link
- if you want to add commandline parameters click Edit Config => Server Start Param
  - ? parameters belong to the begining without space, - parameters with space at the end

### Official Documentation
🗃️ https://steamcommunity.com/sharedfiles/filedetails/?id=2951532944

### The Game
🕹️ https://store.steampowered.com/app/970300/Repoly/

### Dedicated server info
🖥️ https://steamdb.info/app/1189160

## Requirements
[WindowsGSM](https://github.com/WindowsGSM/WindowsGSM) >= 1.21.0

## Installation
1. Download the [latest](https://github.com/raziel7893/WindowsGSM.Repoly/releases/latest) release
1. Move **Repoly.cs** folder to **plugins** folder or import the zip from the plugins tab
1. Click the **[RELOAD PLUGINS]** button or restart WindowsGSM

### Files To Backup
- Save Gane
  - WindowsGSM\servers\%ID%\serverfiles\Repoly\Saved
  - WindowsGSM\servers\%ID%\serverfiles\Repoly\Config
- WindowsGSM Config
  - WindowsGSM\servers\%ID%\configs

### Port Forwarding (YOU NEED THIS, TO BE ABLE TO CONNECT FROM THE INTERNET(only for servers/pcs at home):
- If You don't know How: portforward.com
- 7777 UDP - Default Game Port
- 27015 UDP - Default Query

### Not having an full IPv4 adress ( named CCNAT or DSL Light )
No game or gameserver supports ipv6 only connections. 
- You need to either buy one (most VPN services provide that option. A pal uses ovpn.net for his server, I know of nordvpn also providing that. Should both cost around 7€ cheaper half of it, if your already having an VPN)
- Or you pay a bit more for your internet and take a contract with full ipv4. (depending on your country)
- There are also tunneling methods, which require acces to a server with a full ipv4. Some small VPS can be obtained, not powerfull enough for the servers themself, but only for forwarding. I think there are some for under 5€), the connection is then done via wireguard. but its a bit configuration heavy to setup) 

Or you connect your friends via VPN to your net and play via local lan then.
Many windowsgsm plugin creators recommend zerotier (should be a free VPN designated for gaming) , see chapter below (or tailscale, but no howto there)

## How can you play with your friends without port forwarding?
- Use [zerotier](https://www.zerotier.com/) folow the basic guide and create network
- Download the client app and join to your network
- Create static IP address for your host machine
- Edit WGSM IP Address to your recently created static IP address
- Give your network ID to your friends
- After they've joined to your network
- They can connect using the IP you've created eg: 10.123.17.1:7777
- Enjoy

### Give Love!
[Buy me a coffee](https://ko-fi.com/raziel7893)

[Paypal](https://paypal.me/raziel7893)


### Support
[WGSM](https://discord.com/channels/590590698907107340/645730252672335893)

### License
This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/Soulflare3/WindowsGSM.Repoly/blob/master/LICENSE) file for details
