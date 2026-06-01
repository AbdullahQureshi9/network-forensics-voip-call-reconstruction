VoIP Network Forensics and Call Reconstruction using Wireshark
Overview

This project demonstrates forensic analysis of Voice over IP (VoIP) communications using Wireshark.

The objective was to capture VoIP traffic, analyze SIP and RTP packets, reconstruct audio streams, evaluate call quality, and identify security risks associated with unencrypted VoIP communications.

Developed as part of the Computer Network Forensics course at Laurentian University.

Technologies Used
Wireshark
Linphone
SIP Protocol
RTP Protocol
VoIP.ms
Packet Analysis
Network Forensics
Project Objectives
Capture VoIP traffic
Filter SIP and RTP packets
Extract caller and receiver information
Analyze call quality
Reconstruct audio streams
Identify security vulnerabilities

These objectives were defined during the project planning phase.

Workflow
Configure VoIP environment using Linphone
Capture network traffic using Wireshark
Apply SIP and RTP filters
Analyze call setup and signaling
Extract caller/callee information
Analyze RTP streams
Reconstruct call audio
Perform security assessment
Key Findings
Call Reconstruction

Successfully reconstructed VoIP conversations using RTP stream analysis.

Call Quality Analysis

Measured:

Packet Loss
Jitter
Latency

The project identified increased jitter and latency in certain RTP streams.

Security Assessment

Observed risks:

Eavesdropping
Unencrypted communications
Call tampering potential

Recommended:

SRTP
TLS for SIP signaling

Results

The project successfully:

Captured SIP traffic
Captured RTP streams
Extracted call metadata
Reconstructed audio
Evaluated call quality
Assessed security risks

Repository Contents
Documentation
Presentation Slides
Packet Capture (.pcapng)
Diagrams and Architecture
Analysis Results
Team Members
Hafiz Muhammad Abdullah Qureshi
Prabha Basnet
Liying Cao
Future Enhancements
Automated forensic analysis using Python
AI-assisted VoIP investigation
Large-scale packet analysis
Enhanced attack detection mechanisms
