Objective

Assess OTP identity tracking.

Vulnerability Overview

User-controlled tracking values influenced OTP workflow.

Tactical Mindset

Authentication state must live on server-side sessions.

Methodology

Analyze tracking values and identity flow.

Key Observation

Identity linkage relied on client-controlled data.

Security Impact

Could allow account compromise.

Defensive Fix

Use server-side session identifiers.

Key Learning

Client input should never define identity.
