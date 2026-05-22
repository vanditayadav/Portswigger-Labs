Objective

Analyze password reset token validation.

Vulnerability Overview

Reset workflow improperly validates ownership of reset tokens.

Tactical Mindset

The server must verify that reset credentials belong to the requesting user.

Methodology

Trigger reset.

Observe token behavior.

Test parameter modifications.

Analyze verification logic.

Key Observation

Token validation logic did not correctly bind user identity.

Security Impact

Can lead to account takeover.

Defensive Fix

Bind tokens to sessions/users

Verify ownership server-side

Key Learning

Never trust user-controlled reset parameters.
