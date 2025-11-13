# OSI Model in Practice

## Mapping OSI to TCP/IP Model
Although OSI is conceptual, most real-world networks use TCP/IP. Here’s how they map:
| OSI Model | TCP/IP Model |
| --- | --- |
| Application(7) | Application |
| Presentation(6) | Application |
| Session(5) | Application |
| Transport(4) | Transport |
| Network(3) | Internet |
| Data Link(2) | Network Access |
| Physical(1) | Network Access |

Key Insight: TCP/IP combines Session, Presentation, and Application into one layer.

## How Engineers Use OSI for Troubleshooting
- Layer 1 Issues: Cable unplugged, damaged connectors.
- Layer 2 Issues: MAC address conflicts, VLAN misconfigurations.
- Layer 3 Issues: Wrong IP address, routing problems.
- Layer 4 Issues: Port blocked by firewall, TCP handshake failure.
- Layer 7 Issues: DNS errors, HTTP 404/500 errors.
Practical Tip: When troubleshooting, start from Layer 1 upward (physical check first).

## Real-World Scenarios
- Scenario 1: Website not loading
  - Check Layer 7 (HTTP), Layer 4 (TCP ports), Layer 3 (IP connectivity).
- Scenario 2: VoIP call drops
  - Check Layer 4 (UDP reliability), Layer 3 (routing), Layer 2 (Wi-Fi interference).
- Scenario 3: Slow file transfer
  - Check Layer 4 (TCP congestion), Layer 2 (switch errors), Layer 1 (cable quality).
