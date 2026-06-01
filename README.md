# VoIP Network Forensics and Call Reconstruction using Wireshark

## Overview

This project demonstrates forensic analysis and reconstruction of Voice over IP (VoIP) communications using Wireshark. The project focuses on capturing and analyzing SIP and RTP traffic, reconstructing audio streams, evaluating call quality, and identifying security risks associated with unencrypted VoIP communications.

Developed as part of the Computer Network Forensics course at Laurentian University.

---

## Project Objectives

* Capture VoIP traffic using Wireshark
* Filter SIP and RTP packets
* Extract caller and receiver information
* Analyze call quality metrics
* Reconstruct audio from RTP streams
* Identify security vulnerabilities in VoIP communications
* Recommend security improvements and encryption methods

---

## Technologies Used

* Wireshark
* Linphone
* VoIP.ms
* SIP (Session Initiation Protocol)
* RTP (Real-Time Transport Protocol)
* Network Packet Analysis
* Digital Forensics

---

## Project Workflow

1. Configure VoIP environment using Linphone and VoIP accounts.
2. Capture network traffic using Wireshark.
3. Apply SIP and RTP filters.
4. Extract caller and receiver information.
5. Analyze call setup and signaling.
6. Inspect RTP streams and call quality.
7. Reconstruct audio from captured RTP packets.
8. Perform security assessment and identify vulnerabilities.

---

## Network Architecture

The forensic workflow consists of:

* VoIP Caller
* SIP Server
* Internet Network
* Router
* VoIP Receiver
* Wireshark Packet Capture and Analysis

Wireshark captures and analyzes SIP signaling traffic and RTP media streams to reconstruct and investigate VoIP communications.

---

## Key Features

### SIP Analysis

* Captured SIP signaling traffic
* Analyzed INVITE, ACK, BYE, and response messages
* Extracted caller and receiver metadata

### RTP Analysis

* Captured RTP media streams
* Evaluated packet delivery and stream quality
* Inspected voice traffic transmission

### Call Quality Assessment

Measured:

* Packet Loss
* Jitter
* Latency

### Audio Reconstruction

* Reconstructed audio streams from RTP packets
* Verified voice communication playback using Wireshark's VoIP tools

### Security Assessment

Identified potential risks including:

* Eavesdropping
* Unencrypted VoIP traffic
* Call tampering risks
* Information leakage

Recommended mitigations:

* Secure RTP (SRTP)
* TLS for SIP signaling
* Encrypted VoIP communication channels

---

## Results

### Successful Outcomes

* Captured and analyzed SIP traffic
* Captured and analyzed RTP streams
* Extracted call metadata
* Reconstructed VoIP audio
* Evaluated call quality metrics
* Identified security vulnerabilities

### Limitations

* Some RTP streams contained incomplete audio
* Analysis accuracy depended on complete packet capture
* Limited codec support for certain VoIP implementations

---

## Skills Demonstrated

* Network Forensics
* Cybersecurity Fundamentals
* Packet Analysis
* Wireshark
* VoIP Technologies
* SIP and RTP Analysis
* Security Assessment
* Technical Documentation

---

## Future Improvements

* Python-based automation for forensic analysis
* AI-assisted packet investigation
* Large-scale VoIP traffic analysis
* Advanced attack detection mechanisms
* Automated reporting and visualization
