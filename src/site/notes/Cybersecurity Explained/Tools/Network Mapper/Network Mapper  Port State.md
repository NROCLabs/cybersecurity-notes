---
{"dg-publish":true,"permalink":"/cybersecurity-explained/tools/network-mapper/network-mapper-port-state/","tags":["cybersec","networking","hackthebox","gardenEntry"]}
---

[[Cybersecurity Explained/Tools/Network Mapper/Network Mapper  Scanning Active Ports\|Network Mapper  Scanning Active Ports]]
[[Network Mapper (NMAP)  Introduction \|Network Mapper (NMAP)  Introduction ]]

# The Six States of a Port

| **State**          | **Description**                                                                                                                                            |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `open`             | Connection to the scanned port has been established. These connections can be **TCP Connections**, **UDP Connections**, or `SCTP associations`             |
| `closed`           | The **TCP Protocol** indicates that packet we received contains an `RST` flag. This scanning method can be useful to indicate if the port is alive or not. |
| `filtred`          | Nmap cannot correctly identity if the scanned port is opened or closed. This caused by ether no response or an error code.                                 |
| `unfiltred`        | This state only occurs during a `TCP-ACK` scan. Port is accessible but it cannot be determined if its open or closed.                                      |
| `open -  filtred ` | No response, Nmap will set the port to that state. Indicates a firewall packet filter might be protecting the port.                                        |
| `closed - filtred` | This state only occurs in the `IP ID idle` scans, and indicates it's impossible to determine the scanned port is closed or filtered by a firewall.         |
