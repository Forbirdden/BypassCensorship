# BypassCensorship
My collection of ways to bypass internet censorship/blocking

## VPN
### Ready solutions
| Name       | Protocol        | Free  | OS                      | My review                        | Site                           | Mirror                                                                                                                                   |
|------------|-----------------|-------|-------------------------|----------------------------------|--------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
| AmneziaVPN | AmneziaWG       | 50/50 | Android/iOS/MacOS       | 5/10 Works only on certain sites | [Click](https://amnezia.org)   | [Google](https://amnezia.org/https://storage.googleapis.com/amnezia/amnezia.org) [GitHub](https://github.com/amnezia-vpn/amnezia-client) |
| ProtonVPN  | Stealth/WG/OVPN | 50/50 | Android/iOS/MacOS/Linux | 10/10 Fast, no ads, secure               | [Click](https://protonvpn.com) | [GitHub](https://github.com/ProtonVPN)                                                                                                   |
| PsiphonVPN | LI/SSH/WP       | 50/50 | Android/Win/iOS/Mac     | 7/10 Fast, slow connecting       | [Click](https://psiphon.ca)    | [GitHub](https://github.com/Psiphon-Inc)                                                                                                 |
| Orbot      | Tor             | ✅     | Android/iOS/Mac         | 9/10 Fast, needs Tor bridges     | [Click](https://orbot.app)     | [GitHub](https://github.com/guardianproject) [GitLab](https://gitlab.com/guardianproject)                                                |

### My solutions
| Name              | Description                                                                                                                                                    |
|-------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ProtonOverAmnezia | Connect to Proton using WG confings on their [site](https://protonvpn.com) and "Obfuscate WG" setting in AmneziaVPN                                            |
| ProtonOverAWG     | Connect to Proton using WG confings on their [site](https://protonvpn.com) and modifying setting in native AWG client (JC = 3 or 4 or 5, Jmin = 40, Jmax = 70) |

### README
VPN - Virtual Private Network

AWG - AmneziaWG VPN protocol, fork of WG with DPI protection

WG - WireGuard VPN protocol

DPI - Deep Packet Inspection, used for censoring/blocking internet access

Stealth - VPN protocol made by Proton

OVPN - OpenVPN protocol

Li - L2TP over IPSec

L2TP - Layer 2 Tunneling (VPN) Protocol

IPsec - Internet Protocol Security

SSH - Secure Shell protocol

WP - Web Proxy

Tor - The Onion Router, private network

Onion routing - technique for anonymous communication over a computer network

AmneziaVPN client - modern client for most VPN protocols

AmneziaWG native client - WG client modifyed to work with AWG

