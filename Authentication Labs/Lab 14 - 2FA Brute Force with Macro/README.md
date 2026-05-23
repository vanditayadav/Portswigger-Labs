Goal

Understand how automation affects authentication systems.

My First Thought

Repeated failures should stop brute force attempts.

The Main Idea

Humans become slow when repeating many steps.

Automation removes that difficulty.

What I Tried

Observed repeated login behavior and session flow.

What I Noticed

Fresh sessions allowed continuous attempts.

Why I Changed My Thinking

Instead of focusing only on OTP values, I looked at the whole workflow.

Why It Worked

Automation recreated the required steps repeatedly.

Impact

Can weaken OTP security

Fix

- Limit how many OTP attempts a user can make in a short time.

- Lock or temporarily pause verification after multiple failed attempts.

- Create a new OTP after repeated failures.

- Expire old sessions and tokens quickly.

- Monitor unusual repeated activity that looks automated.

The goal is not only to protect the OTP itself, but also the entire login workflow around it.

What I Learned

Before this lab, I mostly thought security depended on strong passwords or strong OTP codes.

This lab showed me that the process around security matters too.

Even if OTP is strong, automation can repeatedly perform actions much faster than humans.

I learned that attackers do not only attack values like passwords or codes — they also attack workflows and repeated processes.
