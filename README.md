# BypassCensorship
My collection of ways to bypass internet censorship/blocking

## VPN
### Ready solutions
| Name       | Protocol        | Free  | OS                      | My review                        | Site                           | Mirror                                                                                                                                   |
|------------|-----------------|-------|-------------------------|----------------------------------|--------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
| AmneziaVPN | AmneziaWG       | 50/50 | Android/Win/iOS/MacOS/Linux       | 5/10 Works only on certain sites | [Click](https://amnezia.org)   | [Google](https://amnezia.org/https://storage.googleapis.com/amnezia/amnezia.org) [GitHub](https://github.com/amnezia-vpn/amnezia-client) |
| ProtonVPN  | Stealth/WG/OVPN | 50/50 | Android/Win/iOS/MacOS/Linux | 10/10 Fast, no ads, secure               | [Click](https://protonvpn.com) | [GitHub](https://github.com/ProtonVPN)                                                                                                   |
| PsiphonVPN | LI/SSH/WP       | 50/50 | Android/Win/iOS/Mac     | 7/10 Fast, slow connecting       | [Click](https://psiphon.ca)    | [Click](https://psiphon3.com) [GitHub](https://github.com/Psiphon-Inc)                                                                                                 |
| Orbot      | Tor             | ✅     | Android/iOS/Mac         | 9/10 Fast, needs Tor bridges     | [Click](https://orbot.app)     | [GitHub](https://github.com/guardianproject) [GitLab](https://gitlab.com/guardianproject)                                               |

### Custom solutions
| Name              | Description                                                                                                                                                    | Free  | OS                      | My review                        |
|-------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------| - | - | - |
| ProtonOverAmnezia | Connect to Proton using WG confings on their [site](https://protonvpn.com) and "Obfuscate WG" setting in AmneziaVPN client                                           | ✅ | Android/iOS/MacOS/Linux | 9/10 |
| ProtonOverAWG     | Connect to Proton using WG confings on their [site](https://protonvpn.com) and modifying settings in native AWG client (JC = 3 or 4 or 5, Jmin = 40, Jmax = 70) | ✅ | Android/iOS/MacOS/Linux | 8/10 |
| WARPoverAWG     | Connect to WARP using config generated using [this bash script](https://raw.githubusercontent.com/ImMALWARE/bash-warp-generator/refs/heads/main/warp_generator.sh) and import to native AWG client | ✅ | Android/iOS/MacOS/Linux | 10/10 |

### Dictionary
```
VPN - Virtual Private Network
AWG - AmneziaWG VPN protocol, fork of WG with DPI protection
WG - WireGuard VPN protocol
DPI - Deep Packet Inspection, used for censoring/blocking internet access
Stealth - VPN protocol made by Proton
OVPN - OpenVPN protocol
LI - L2TP over IPSec
L2TP - Layer 2 Tunneling (VPN) Protocol
IPsec - Internet Protocol Security
SSH - Secure Shell protocol
WP - Web Proxy
Tor - The Onion Router, private network
Onion routing - technique for anonymous communication over a computer network
Tor bridges - Relays that help access the Tor network
AmneziaVPN client - modern client for most VPN protocols
AmneziaWG native client - WG client modifyed to work with AWG
WARP - VPN made by Cloudflare
```
## Other software
### Ready solutions
| Name         | Description                                                                                | Free | OS                          | My review                                                        | Site                                             | Mirror                                                                      |
|--------------|--------------------------------------------------------------------------------------------|------|-----------------------------|------------------------------------------------------------------|--------------------------------------------------|-----------------------------------------------------------------------------|
| GoodbyeDPI   | TCP-only passive DPI blocker and active DPI circumvention utility                          | ✅    | Windows                     | 8/10 Only TCP                                                    | [GitHub](https://github.com/ValdikSS/GoodbyeDPI) |                                                                             |
| Zapret       | TCP/UDP DPI bypass utility                                                                 | ✅    | Windows/Mac/Linux           | 7/10 Doesn't work for me, but got high reviews from other people | [GitHub](https://github.com/bol-van/zapret)      |                                                                             |
| Tor browser  | Web browser that uses TOR network                                                          | ✅    | Android/Win/MacOS/Linux | 8/10 Needs bridges                                               | [Click](https://www.torproject.org)              | [GitHub](https://github.com/TheTorProject/gettorbrowser) [Archive.org](https://archive.org/search?query=creator%3A%22Tor+Project%22)                   |
| Ceno browser | Web browser that uses Ouinet network                                                       | ✅    | Android/Windows             | 8/10 Nice but slow                                               | [Click](https://censorship.no)                   | [GitHub](https://github.com/ceno-app) [GitLab](https://gitlab.com/ceno-app) |
| Paskoocheh   | App store that uses Ouinet network with various anti-internet-censorship/blocking software | ✅    | Android/Win/iOS/MacOS/Linux | 10/10 Awesome                                                    | [Click](https://paskoocheh.com)                  |       
| Onion Browser   | Unofficial Tor browser for iOS, recommended by the Tor Project team | ✅    | iOS | I don`t have an iPhone or iPad                                                    | [Click](https://onionbrowser.com)                  |                                                                         |

### Custom solutions
| Name              | Description                                   | Free | OS      | My review                         |
|-------------------|-----------------------------------------------|------|---------|-----------------------------------|
| GoodbyeDPI+Zapret | Simply launching GDPI and Zapret at same time | ✅    | Windows | 10/10 Finally, Discord with working calls |

### Dictionary
```
DPI - Deep Packet Inspection, used for censoring/blocking internet access
Tor - The Onion Router, private network
Onion routing - technique for anonymous communication over a computer network
Tor bridges - Relays that help access the Tor network
TCP - Transmission Control Protocol
UDP - User Datagram Protocol
Ouinet - BitTorrent based P2P network
```
## Other stuff
### Mirrors
#### GetTor (Tor Browser)
Send an email to gettor@torproject.org In the body of the mail, write the name of your operating system (such as Windows, macOS, or Linux). GetTor will respond with an email containing links from which you can download Tor Browser, the cryptographic signature (needed for verifying the download), the fingerprint of the key used to make the signature, and the package's checksum. You may be offered a choice of "32-bit" or "64-bit" software: this depends on the model of the computer you are using; consult documentation about your computer to find out more. Note that you must send the email using one of the following email providers: Riseup or Gmail
#### Download via Email (PsiphonVPN)
Works similar to GetTor, just send at empty email to get@psiphon3.com
### Tor bridges
#### BridgeDB
https://bridges.torproject.org/options
#### BridgeDB over Email
Send an email to bridges@torproject.org. Leave the subject blank and write "get transport obfs4" in the body. Note that you must send the email using one of the following email providers: Riseup or Gmail
#### ntc.party bridges
https://torscan-ru.ntc.party/
#### GetBridges Telegram bot
https://t.me/GetBridgesBot
#### Tor Relay Scanner (from GoodbyeDPI creator)
https://github.com/ValdikSS/tor-relay-scanner
