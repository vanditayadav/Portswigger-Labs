Tools Used: Browser + Burp

Goal

Check whether OTP protection is actually enforced.

My First Thought

I assumed OTP must always be completed before account access.

The Main Idea

Imagine a mall security guard checks your ticket but forgets to check whether you passed the final gate.

You may still enter.

What I Tried

Logged in and stopped at OTP page.

Instead of entering OTP, I manually changed the URL.

What I Noticed

Protected pages were still opening.

Why I Changed My Thinking

I stopped thinking about OTP numbers.

Instead I wondered:

"Does the website already think I am logged in?"

Why It Worked

The website partly trusted me after password verification.

Impact

Someone with credentials could skip OTP.

Fix

Check OTP completion on server side.

What I Learned

Security sometimes fails because of wrong assumptions.
