# Quick Summary

| Layer | Name           | PDU      | Example/Protocols       |
|-------|---------------|----------|--------------------------|
| 7     | Application   | Data     | HTTP, FTP, SMTP, DNS    |
| 6     | Presentation  | Data     | SSL/TLS, JPEG, MPEG     |
| 5     | Session       | Data     | NetBIOS, RPC, SIP       |
| 4     | Transport     | Segment  | TCP, UDP, SCTP          |
| 3     | Network       | Packet   | IP, ICMP, ARP           |
| 2     | Data Link     | Frame    | Ethernet, PPP, HDLC     |
| 1     | Physical      | Bits     | Cables, Hubs, Fiber     |


## PDU Names
- Application → Data
- Transport → Segment
- Network → Packet
- Data Link → Frame
- Physical → Bits

## Common Protocols by Layer
- Layer 7: HTTP, FTP, SMTP, DNS
- Layer 6: SSL/TLS, JPEG, MPEG
- Layer 5: NetBIOS, RPC
- Layer 4: TCP, UDP
- Layer 3: IP, ICMP, ARP
- Layer 2: Ethernet, PPP
- Layer 1: Physical media (cables, connectors)

## Troubleshooting Approach
- Start at Layer 1: Check cables, connectors.
- Layer 2: Check MAC addresses, VLANs.
- Layer 3: Verify IP addressing and routing.
- Layer 4: Check ports and TCP/UDP connectivity.
- Layer 7: Validate application services (DNS, HTTP).
