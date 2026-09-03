# Cisco Packet Tracer - Secure Wireless Network Configuration

A Cisco Packet Tracer lab demonstrating the configuration, security, and validation of a small wireless LAN.

## Project overview

This project configures a wireless access point (WAP) to provide secure connectivity for a laptop, tablet, and smartphone. The setup uses DHCP for automated addressing, a MAC-based DHCP reservation for the laptop, WPA2-Personal wireless protection, and remote administration of the WAP.

## Objectives completed

- Prepared the laptop for Wi-Fi by using a wireless network module and configuring its MAC address.
- Configured the WAP to obtain a DHCP lease from the ISP.
- Configured LAN DHCP services and a reservation for the laptop MAC address.
- Configured and secured the wireless radios.
- Connected and tested a tablet, smartphone, and laptop.
- Verified DHCP leasing, server browsing, and remote WAP administration.

## LAN DHCP configuration

| Setting | Value |
| --- | --- |
| LAN network | `192.168.0.0/24` |
| WAP LAN / default gateway | `192.168.0.1` |
| DHCP pool start | `192.168.0.100` |
| DNS server | `200.200.200.200` |
| Reservation | Static DHCP lease reserved for the configured laptop MAC address |

The DHCP reservation lets the laptop receive the same assigned IP address whenever it reconnects, while the other clients receive addresses dynamically from the DHCP scope.

## Wireless configuration

| Setting | Value |
| --- | --- |
| SSID | `OurHouse` |
| SSID broadcast | Enabled on all radios |
| 2.4 GHz channel | 11 |
| 5 GHz channel bandwidth | 80 MHz |
| Wireless security | WPA2-Personal |
| Authentication | Pre-shared key (PSK) configured |

> Security note: The actual Wi-Fi PSK and remote-administration password are intentionally not published in this repository.

## WAP administration

- Remote administration was enabled on the WAP.
- A remote-administration password was configured.
- The laptop was used to open a browser connection to the WAP LAN router address and verify remote-management access.

## Validation

The completed configuration was tested by confirming that:

- The laptop, tablet, and smartphone successfully joined the `OurHouse` wireless network.
- Each client received a valid DHCP lease.
- Clients could open a browser connection to the network server.
- The laptop could access the WAP management interface remotely through its LAN router address.


## Skills demonstrated

Cisco Packet Tracer, wireless LAN configuration, DHCP, IP addressing, DHCP reservation, WPA2-Personal, PSK authentication, 2.4 GHz and 5 GHz Wi-Fi configuration, remote administration, and network connectivity testing.
