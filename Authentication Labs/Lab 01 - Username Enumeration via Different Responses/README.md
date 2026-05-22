Tools Used: Burp Suite Intruder

Objective

Understand how different authentication responses reveal valid users.

Vulnerability Overview

The application leaks account existence through inconsistent error messages.

Tactical Mindset

If the application says more than "Invalid credentials," it may accidentally reveal user existence.

Methodology

1.Intercept login request.

2.Send to Intruder.

3.Target username parameter.

4.Use username wordlist.

5.Compare response lengths or Grep-Match.

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
