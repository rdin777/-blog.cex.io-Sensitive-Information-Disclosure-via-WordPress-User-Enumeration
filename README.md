# WordPress User Enumeration PoC (CVE-2017-5487 Logic)

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
