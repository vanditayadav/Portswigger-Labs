Objective

Test JSON parsing abuse.

Vulnerability Overview

Application processed multiple credentials in one request.

Tactical Mindset

Rate limiting often assumes one request equals one attempt.

Methodology

Analyze input structure flexibility.

Key Observation

Arrays bypassed intended logic.

Security Impact

Rate-limit bypass.

Defensive Fix

Validate request schema strictly.

Key Learning

Unexpected formats create unexpected behavior.
