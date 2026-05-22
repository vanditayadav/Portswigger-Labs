Tools Used: Browser + Burp Suite

Objective

Determine whether 2FA is enforced server-side.

Vulnerability Overview

Application creates a partially authenticated session before OTP validation.

Tactical Mindset

Access control must verify authentication state, not assume workflow completion.

Methodology

1.Login normally.

2.Reach OTP page.

3.Change destination URL.

4.Attempt direct access.

Key Observation

Protected resources were accessible without OTP completion.

Security Impact

2FA protection becomes ineffective.

Defensive Fix

Verify 2FA server-side

Block access before verification completion

Key Learning

Authentication flow logic matters as much as authentication itself.
