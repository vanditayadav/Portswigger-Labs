Platform: PortSwigger Web Security Academy

Category: Authentication

Tools Used: Burp Suite Intruder

Objective

Understand how different authentication responses reveal valid users.

Vulnerability Overview

The application leaks account existence through inconsistent error messages.

Tactical Mindset

If the application says more than "Invalid credentials," it may accidentally reveal user existence.

Methodology

Intercept login request.

Send to Intruder.

Target username parameter.

Use username wordlist.

Compare response lengths or Grep-Match.

Key Observation

A valid username produced a structurally different response.

Security Impact

User enumeration reduces attack effort and enables targeted brute forcing.

Defensive Fix

Use generic authentication messages

Normalize responses

Apply rate limiting

Key Learning

Small response differences create major information leaks.
