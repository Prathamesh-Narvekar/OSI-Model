# Layer 6: Presentation Layer

## Role and Responsibilities
- Acts as the translator between the application layer and the network.
- Ensures that data is in a format understandable by both sender and receiver.
- Handles data encryption, compression, and encoding.

## Key Functions
- Data Translation: Converts data from application format to network format (and vice versa).
- Encryption & Decryption: Secures data during transmission.
- Compression: Reduces data size for faster transmission.
- Character Encoding: Converts between ASCII, Unicode, etc.

## Devices at Presentation Layer
(Mostly software-based, not hardware-specific)
- Encryption Gateways: Devices or software that encrypt/decrypt data.
- SSL/TLS Accelerators: Hardware or software for secure communication.

## Standards & Protocols
- SSL/TLS: Secure communication for web traffic.
- JPEG, GIF, PNG: Image encoding standards.
- MPEG: Video compression standard.
- ASCII, Unicode: Text encoding standards.

## Common Issues
- Encoding Mismatch: Sender uses Unicode, receiver expects ASCII.
- Encryption Errors: SSL/TLS handshake failures.
- Compression Problems: Data corruption during compression/decompression.
- Certificate Issues: Invalid or expired SSL certificates.

## Real-World Examples
- HTTPS websites using SSL/TLS for secure communication.
- Image and video streaming using JPEG/MPEG formats.
- Text files encoded in UTF-8 for global compatibility.
