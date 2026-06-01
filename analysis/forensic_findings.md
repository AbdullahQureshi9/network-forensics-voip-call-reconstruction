# Forensic Findings and Analysis

## Project Overview

This project focused on the forensic analysis of Voice over IP (VoIP) communications using Wireshark. The objective was to investigate captured network traffic, identify VoIP signaling and media streams, reconstruct audio communications, evaluate call quality, and assess security vulnerabilities associated with VoIP systems.

The investigation was performed using packet captures generated from VoIP calls established through Linphone and analyzed using Wireshark.

---

# Investigation Methodology

The forensic investigation followed a structured workflow:

1. Configure the VoIP environment.
2. Establish a voice call between two endpoints.
3. Capture network traffic using Wireshark.
4. Apply protocol filters to isolate VoIP traffic.
5. Analyze SIP signaling messages.
6. Analyze RTP media streams.
7. Reconstruct call audio.
8. Evaluate call quality metrics.
9. Perform security assessment.

This methodology follows common digital forensics practices for VoIP investigations.

---

# SIP Analysis Findings

Session Initiation Protocol (SIP) packets were examined to identify communication participants and call setup procedures.

The following SIP messages were observed:

* INVITE
* TRYING
* RINGING
* OK (200)
* ACK
* BYE

These messages confirmed successful call establishment, maintenance, and termination.

### Key Observations

* Caller and receiver information was successfully identified.
* Call setup followed the expected SIP signaling sequence.
* No abnormal SIP responses were detected.
* No evidence of SIP-based attacks was observed during testing.

---

# RTP Stream Analysis

Real-Time Transport Protocol (RTP) streams were analyzed to investigate media transmission.

The RTP streams contained the voice payload exchanged between the communicating parties.

### Key Findings

* RTP streams were successfully identified.
* Voice packets were transmitted continuously during active communication.
* Sequence numbers were generally consistent.
* Packet delivery remained stable throughout most of the call.

The RTP analysis confirmed successful voice transmission between endpoints.

---

# Call Quality Assessment

Several metrics were reviewed to evaluate communication quality.

### Packet Loss

Packet loss remained extremely low during testing.

Impact:

* Minimal audio degradation.
* Stable communication quality.

### Jitter

Jitter values exceeded recommended thresholds during certain portions of the call.

Impact:

* Potential voice distortion.
* Delayed packet arrival.
* Reduced user experience.

### Latency

Latency values were also observed above recommended levels.

Impact:

* Possible delays during conversation.
* Reduced real-time communication quality.

Overall, the call remained functional despite these quality concerns.

---

# Audio Reconstruction

One of the primary objectives of this investigation was the reconstruction of voice communications.

Using Wireshark's VoIP analysis tools:

* RTP streams were extracted.
* Audio playback functionality was utilized.
* Voice communication was successfully reconstructed.

This demonstrates how network packet captures can be used to recover communication content when VoIP traffic is not encrypted.

---

# Security Assessment

The investigation identified several security concerns associated with unencrypted VoIP communications.

## Risk 1: Eavesdropping

Attackers who gain access to network traffic may be able to:

* Capture SIP packets
* Capture RTP streams
* Reconstruct conversations

This represents a significant privacy concern.

## Risk 2: Information Disclosure

SIP messages may expose:

* Caller identifiers
* Receiver identifiers
* Call metadata
* Network information

Such information may assist attackers in reconnaissance activities.

## Risk 3: Call Tampering

Unsecured VoIP systems may be vulnerable to:

* Session hijacking
* Packet manipulation
* Call interception

Although these attacks were not observed during testing, the risk remains present in unencrypted environments.

---

# Security Recommendations

Based on the findings, the following improvements are recommended:

## Secure RTP (SRTP)

Encrypt RTP streams to prevent unauthorized audio reconstruction.

Benefits:

* Confidentiality
* Integrity
* Protection against eavesdropping

## Transport Layer Security (TLS)

Use TLS to secure SIP signaling traffic.

Benefits:

* Secure call setup
* Protected metadata
* Reduced interception risk

## Network Monitoring

Implement continuous monitoring using:

* Wireshark
* IDS/IPS systems
* Security logging tools

This improves detection of abnormal VoIP activity.

---

# Skills Demonstrated

This project helped develop practical skills in:

* Network Forensics
* Packet Analysis
* Wireshark
* VoIP Technologies
* SIP Analysis
* RTP Analysis
* Digital Investigations
* Security Assessment
* Technical Documentation

---

# Personal Reflection

Through this project, I gained hands-on experience in analyzing network traffic and understanding how voice communications operate over IP networks.

I learned how to:

* Capture and inspect network packets.
* Trace VoIP call establishment processes.
* Analyze RTP media streams.
* Reconstruct voice communications.
* Evaluate communication quality.
* Assess security risks within network environments.

This project strengthened my interest in cybersecurity, digital forensics, and network security, and provided practical exposure to real-world forensic investigation techniques.
