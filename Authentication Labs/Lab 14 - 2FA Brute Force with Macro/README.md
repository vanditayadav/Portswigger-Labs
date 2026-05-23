Tool: Macro + Intruder

Goal

Understand how automation affects authentication systems.

My First Thought

Repeated failures should stop brute force attempts.

The Main Idea

Humans become slow when repeating many steps.

Automation removes that difficulty. Here comes Macro.

What is a Macro?

A macro is a way to automate a sequence of repeated actions.

Instead of manually doing the same steps again and again, the tool performs them automatically in the same order.

In this lab, the website required multiple steps before reaching the OTP page:

- Login

- Create a session

- Get fresh values/tokens

- Reach OTP verification

Doing this manually for every OTP guess would be slow.

So a macro repeated these steps automatically before each new attempt.

Think of it like recording a small routine:

Step 1 → Step 2 → Step 3 → repeat automatically

This saves time and allows testing to continue smoothly.

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
