# Introduction to OSI Model

<div align = center>
<img width="800" height="500" alt="image" src="https://github.com/user-attachments/assets/3505ee1e-1025-4c1a-9241-ca110f7aa2b9" />
</div>

## What is the OSI Model?
The OSI (Open Systems Interconnection) Model is a conceptual framework developed by the International Organization for Standardization (ISO). It standardizes how different networking systems communicate over a network by dividing the communication process into seven distinct layers. Each layer has specific responsibilities and interacts with the layers directly above and below it.	

## Purpose of the OSI Model
- Standardization: Provides a universal set of rules for network communication.
- Interoperability: Ensures different hardware and software systems can work together.
- Troubleshooting: Helps network engineers isolate problems by layer.
- Modularity: Allows upgrades or changes in one layer without affecting others.

## Why is OSI Important?
- It serves as a reference model for designing and understanding network protocols.
- It helps in protocol development, network design, and problem-solving.
- Even though modern networks often use the TCP/IP model, OSI remains crucial for learning and conceptual clarity.

## OSI vs TCP/IP Model
| Feature | OSI Model (7 Layers) | TCP/IP Model (4 Layers) |
| --- | --- | --- |
| Layers | Physical, Data Link, Network, Transport, Session, Presentation, Application | Network Interface, Internet, Transport, Application |
| Developed By | ISO | DARPA (for ARPANET) |
| Usage | Conceptual Framework | Practical Implementation |

## Limitations of OSI Model
- Too theoretical: It was never fully implemented in real networks.
- Complexity: Seven layers can be overkill for practical use.
- TCP/IP became dominant: Because it was simpler and adopted early by ARPANET.

## Real-World Analogy
Think of sending a letter via postal service:
- Application Layer: You write the letter (content).
- Presentation Layer: You format it (language, encoding).
- Session Layer: You decide when to send and receive (conversation control).
- Transport Layer: You ensure delivery (reliable or not).
- Network Layer: You choose the route (addressing).
- Data Link Layer: You put it in an envelope (framing).
- Physical Layer: The mail truck physically carries it (medium).

## Key Concepts
- Encapsulation: Wrapping data with protocol information as it moves down layers.
- Decapsulation: Removing protocol information as data moves up layers.
- PDU (Protocol Data Unit): The name of data at each layer (e.g., Frame, Packet, Segment).
