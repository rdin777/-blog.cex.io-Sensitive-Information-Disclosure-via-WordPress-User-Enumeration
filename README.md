# WordPress User Enumeration PoC (CVE-2017-5487 Logic)

*If this research helped you, please consider giving it a ⭐ Star.*


## 🚀 Stay Updated
Found this research useful?
* **Star ⭐** this repo to keep track of it.
* **Follow me** on GitHub for more DeFi security research.
* **Fork** it if you want to run your own experiments.

### ☕ Support the Research
If you appreciate the work and want to support further security research:

<img src="456.PNG" alt="Donate QR" width="200"/>

**Wallet Address (ETH/EVM):** 0xBDDD7973D0DE27B715A4A5cbdb87d0DF78757b3A 


This repository contains a simple Proof of Concept (PoC) script for enumerating users via the WordPress REST API.

## Description
WordPress versions with enabled REST API often expose the `/wp-json/wp-v2/users` endpoint. If not properly restricted, this allows unauthenticated attackers to gather a list of valid usernames and IDs.

**Impact:**
- **Brute-Force Attacks:** Attackers gain valid login names.
- **Social Engineering:** Knowing real names of employees allows for targeted phishing.

## Usage
```bash
pip install -r requirements.txt
python exploit.py
