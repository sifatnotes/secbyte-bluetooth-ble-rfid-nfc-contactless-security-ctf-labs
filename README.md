# secbyte-bluetooth-ble-rfid-nfc-contactless-security-ctf-labs
A practical collection of cybersecurity CTF labs covering Bluetooth Classic &amp; Low Energy (BLE) security (packet sniffing, pairing attacks, GATT enumeration, trust collapse, BlueBeacon breaches) and contactless physical/wireless security (RFID badge replay, access card assessments, NFC payment manipulation, RFID reader investigation).
# Bluetooth Classic, BLE Sniffing, RFID Badge Replay & NFC Contactless Security CTF Labs

Welcome to the **Bluetooth Classic, BLE Sniffing, RFID Badge Replay & NFC Contactless Security CTF Lab Collection**. This repository serves as an organized, searchable catalog of practical cybersecurity labs hosted on Learn SecByte.

This collection focuses on short-range RF communications, wireless protocol analysis, and physical security access controls—spanning **Bluetooth BR/EDR & BLE Protocol Analysis (Sniffing, GATT service discovery, packet sleuthing, device triage)**, **Bluetooth Trust Abuse & Exploitation (Shattered pairing, silent pairing trust collapse, BlueSilence attacks, BlueBeacon breaches)**, **RFID Security & Physical Access Cards (Badge replay, low/high-frequency badge cloning, access card assessments, reader investigations)**, and **NFC Security & Contactless Payment Systems (Contactless lab, tap-and-pay transaction manipulation)**.

---

## Lab Collection Index

### 1. Bluetooth & BLE Protocol Analysis & Device Enumeration
* **Bluetooth Fundamentals: The BlueBeacon Breach**  
  *Lab Link:* [https://learn.secbyte.org/ctf/bluetooth-fundamentals-the-bluebeacon-breach](https://learn.secbyte.org/ctf/bluetooth-fundamentals-the-bluebeacon-breach)  
  *Focus:* Core principles of Bluetooth architecture (BR/EDR vs. BLE), capturing advertising channels (37, 38, 39), analyzing iBeacon/Eddystone frame structures, and identifying rogue beacon placement.

* **Bleeding Blueprints: BLE Device Enumeration**  
  *Lab Link:* [https://learn.secbyte.org/ctf/bleeding-blueprints-ble-device-enumeration](https://learn.secbyte.org/ctf/bleeding-blueprints-ble-device-enumeration)  
  *Focus:* Mapping Generic Attribute Profile (GATT) services and characteristics using `gatttool`/`bluetoothctl`, reading/writing unencrypted handles, and identifying exposed device interfaces.

<Image src="image_agent_tag_14983218464731310193" alt="Bluetooth Core Architecture showing Host, Controller, and LE/BR/EDR configurations" caption="Bluetooth Host & Controller Architecture Overview" />

---

* **Bluetooth Packet Sleuthing**  
  *Lab Link:* [https://learn.secbyte.org/ctf/bluetooth-packet-sleuthing](https://learn.secbyte.org/ctf/bluetooth-packet-sleuthing)  
  *Focus:* Analyzing PCAP captures containing L2CAP, ATT, and SMP layers with Wireshark; decoding opcode commands; and extracting sensitive payloads transmitted over airwaves.

* **Blue-Echo: BLE Device Triage**  
  *Lab Link:* [https://learn.secbyte.org/ctf/blue-echo-ble-device-triage](https://learn.secbyte.org/ctf/blue-echo-ble-device-triage)  
  *Focus:* Triaging vulnerable BLE IoT endpoints, sniffing connection handshakes, identifying missing encryption requirements, and analyzing device state changes.

### 2. Bluetooth Pairing Exploitation & Trust Subversion
* **Bluetooth Sniffing: The Shattered Pairing**  
  *Lab Link:* [https://learn.secbyte.org/ctf/bluetooth-sniffing-the-shattered-pairing](https://learn.secbyte.org/ctf/bluetooth-sniffing-the-shattered-pairing)  
  *Focus:* Intercepting over-the-air pairing procedures, cracking legacy PINs / Just Works security models, deriving Long Term Keys (LTK), and decrypting captured sessions.

* **Silent Pairing: Bluetooth Trust Collapse**  
  *Lab Link:* [https://learn.secbyte.org/ctf/silent-pairing-bluetooth-trust-collapse](https://learn.secbyte.org/ctf/silent-pairing-bluetooth-trust-collapse)  
  *Focus:* Exploiting silent pairing flaws in Bluetooth HID peripherals, bypassing user confirmation prompts, and injecting malicious keystrokes via unauthorized trust associations.

* **BlueSilence: Bluetooth Trust Abuse**  
  *Lab Link:* [https://learn.secbyte.org/ctf/bluesilence-bluetooth-trust-abuse](https://learn.secbyte.org/ctf/bluesilence-bluetooth-trust-abuse)  
  *Focus:* Executing impersonation attacks against paired Bluetooth trusted devices, forcing downgrade re-pairing routines, and hijacking active device connections.

### 3. RFID Security, Badge Replay & Physical Access Cards
* **RFID Replay: The Badge That Opened the Door**  
  *Lab Link:* [https://learn.secbyte.org/ctf/rfid-replay-the-badge-that-opened-the-door](https://learn.secbyte.org/ctf/rfid-replay-the-badge-that-opened-the-door)  
  *Focus:* Sniffing low-frequency (125 kHz) and high-frequency (13.56 MHz) badge signals, capturing raw ID streams, and performing replay attacks to bypass physical locks.

<Image src="image_agent_tag_14983218464731309896" alt="Diagram of an Electronic Access Control System with controller, reader, and electronic lock" caption="Electronic Access Control System Architecture" />

---

* **Access Card Assessment**  
  *Lab Link:* [https://learn.secbyte.org/ctf/access-card-assessment](https://learn.secbyte.org/ctf/access-card-assessment)  
  *Focus:* Evaluating card technologies (EM4100, HID Prox, MIFARE Classic), extracting keys using nested/darkside attacks, and analyzing sector data structures.

* **RFID Reader Investigation: Station 7**  
  *Lab Link:* [https://learn.secbyte.org/ctf/rfid-reader-investigation-station-7](https://learn.secbyte.org/ctf/rfid-reader-investigation-station-7)  
  *Focus:* Analyzing physical RFID reader controller communication (Wiegand protocol, OSDP), detecting hardware implant taps, and triaging reader firmware vulnerabilities.

### 4. Contactless Security & NFC Payment Systems
* **Contactless Security Lab**  
  *Lab Link:* [https://learn.secbyte.org/ctf/contactless-security-lab](https://learn.secbyte.org/ctf/contactless-security-lab)  
  *Focus:* Fundamentals of Near Field Communication (NFC) protocols (ISO/IEC 14443, NDEF formats), reading tag contents, and auditing contactless reader fields.

* **Tap, Pay, Misbehave: NFC Payment Security**  
  *Lab Link:* [https://learn.secbyte.org/ctf/tap-pay-misbehave-nfc-payment-security](https://learn.secbyte.org/ctf/tap-pay-misbehave-nfc-payment-security)  
  *Focus:* Auditing EMV contactless payment flows, analyzing transaction data exchanges (APDU commands), identifying pre-replay flaws, and testing POS terminal guardrails.

---

## Learning Path

### Path A: Bluetooth & BLE Security Specialist
1. **Fundamentals & Enumeration:** Start with [Bluetooth Fundamentals](https://learn.secbyte.org/ctf/bluetooth-fundamentals-the-bluebeacon-breach), [Bleeding Blueprints](https://learn.secbyte.org/ctf/bleeding-blueprints-ble-device-enumeration), and [Bluetooth Packet Sleuthing](https://learn.secbyte.org/ctf/bluetooth-packet-sleuthing).
2. **Pairing & Trust Exploitation:** Master pairing attacks in [Bluetooth Sniffing: The Shattered Pairing](https://learn.secbyte.org/ctf/bluetooth-sniffing-the-shattered-pairing), [Silent Pairing: Trust Collapse](https://learn.secbyte.org/ctf/silent-pairing-bluetooth-trust-collapse), and [BlueSilence: Trust Abuse](https://learn.secbyte.org/ctf/bluesilence-bluetooth-trust-abuse).

### Path B: RFID & Physical Access Control Specialist
1. **Signal Capture & Replay:** Learn badge mechanics in [RFID Replay: The Badge That Opened the Door](https://learn.secbyte.org/ctf/rfid-replay-the-badge-that-opened-the-door) and [Access Card Assessment](https://learn.secbyte.org/ctf/access-card-assessment).
2. **Hardware & Reader Analysis:** Audit reader infrastructure in [RFID Reader Investigation: Station 7](https://learn.secbyte.org/ctf/rfid-reader-investigation-station-7).

### Path C: NFC & Contactless Systems Auditor
1. **NFC & Payment Testing:** Audit contactless interfaces in [Contactless Security Lab](https://learn.secbyte.org/ctf/contactless-security-lab) and [Tap, Pay, Misbehave: NFC Payment Security](https://learn.secbyte.org/ctf/tap-pay-misbehave-nfc-payment-security).

---

## How to Use the Labs

1. Select a practice scenario from the **Lab Collection Index**.
2. Click the direct link to launch the exercise environment on Learn SecByte.
3. Review scenario directives, Wireshark packet captures (`.pcap`/`.pcapng`), Proxmark3 traces, or raw APDU command logs.
4. Extract GATT characteristics, crack weak Bluetooth PINs, derive MIFARE encryption keys, replay RFID badge signals, or analyze NFC payment APDU frames to capture flags.

---

## Target Audience

* **Wireless Security Researchers & Hardware Pentesters:** Sniff BLE GATT characteristics, analyze Bluetooth pairing handshakes, and test RFID/NFC physical access controllers.
* **Physical Security Auditors & Systems Engineers:** Evaluate badge technology risks (HID Prox vs. MIFARE), audit Wiegand/OSDP reader lines, and assess building entry controls.
* **Payment Security Specialists & Fraud Analysts:** Inspect EMV contactless payment APDU exchanges, audit POS terminal validation rules, and detect NFC replay flaws.
* **Cybersecurity Students:** Acquire hands-on experience with wireless protocols, radio frequency (RF) security concepts, and hardware access control auditing.

---

## Disclaimer

All lab links provided in this repository direct to official training environments hosted on Learn SecByte. All materials and exercises are provided strictly for educational purposes, defensive skill building, and authorized security research. Unauthorized scanning, signal replay, card cloning, or interception against real-world systems without prior authorization is strictly prohibited.
