# Insecure Direct Object Reference (IDOR) Lab

## Overview

This project contains my notes and walkthrough for completing an IDOR vulnerability lab.

The lab demonstrates how insecure direct object references can allow attackers to access unauthorized resources by modifying user-controlled input such as IDs, filenames, or URLs.

---

## What is IDOR?

IDOR (Insecure Direct Object Reference) is an access control vulnerability that occurs when an application exposes internal objects like:

- User IDs
- File names
- Database records
- URLs

without properly verifying authorization.

Example:

```text
https://example.com/profile?id=102
```

An attacker may change the ID value to access another user's data.

---

## Lab Objective

The goal was to identify and exploit an IDOR vulnerability by modifying direct object references.

---

## Steps Performed

1. Logged into the lab environment
2. Intercepted requests and analyzed parameters
3. Identified predictable object references
4. Modified the reference value
5. Accessed unauthorized data
6. Completed the lab successfully

---

## Impact

Successful IDOR attacks can lead to:

- Unauthorized account access
- Exposure of sensitive information
- Data leakage
- Privilege escalation

---

## Mitigation

To prevent IDOR vulnerabilities:

- Implement proper access control checks
- Use indirect object references
- Validate user permissions server-side
- Avoid predictable identifiers

---

## Screenshot

![Lab Completed](screenshots/idor-lab-completed.jpg)

---

## Skills Practiced

- Web application security
- Access control testing
- HTTP request analysis
- Vulnerability assessment

---

## Disclaimer

This project was completed in a legal training environment for educational purposes only.**
