# Erasr - Digital Identity Protection Framework

[![Build status](https://ci.appveyor.com/api/projects/status/5857hfy6r1ltb5f2?svg=true)](https://github.com/rdprs/Erasr)
[![License](https://img.shields.io/github/license/quasar/Quasar.svg)](LICENSE)
![Preview](img/preview.png)

Erasr is a comprehensive anti-stealer framework designed to protect your data by removing all sensitive data, sessions, and files a stealer may target. This data is replaced with convincing decoy information. A secure backup is then created of your personal data in an encrypted format that can be restored when needed, effectively making your system resistant to information-stealing malware.

---

## TECHNICAL ARCHITECTURE

The core of Erasr operates as a data sanitization and protection system that identifies, extracts, secures, and replaces sensitive information across many different applications.

### 1. Data Extraction & Encryption

Erasr systematically scans for and extracts sensitive information from various locations on your system:

**Target Data Types:**
- Cryptocurrency wallet credentials and seed phrases
- Browser sessions and authentication tokens
- Application autofill data and saved passwords
- SSH keys and development credentials
- Personal documents and configuration files

**Encryption Mechanism:**
All extracted data is encrypted using AES-256 encryption and stored in a password-protected `.erasr` file. This file can only be decrypted and restored with the original encryption key, ensuring your data remains secure even if the file is compromised.

### 2. Data Sanitization & Replacement

After secure extraction, Erasr removes all traces of your personal data and replaces it with realistic but fake information:

**Decoy Generation:**
- Creation of cryptocurrency wallets 
- Creation of fake browser history
- Creation of password managers 
- Creation of decoy documents 

---

## Requirements
- Windows 10/11 (x64)
- .NET Framework 4.7.2 or higher
- 36MB of free disk space for the application
- Additional space for encrypted backups (varies based on data volume)

---

## DISCLAIMER
This software is intended for legitimate protection of personal data against unauthorized access. Users are responsible for ensuring they have the right to protect and modify data on their systems. The developers are not responsible for any misuse of this software or data loss resulting from improper use.
