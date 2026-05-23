Goal

Understand how small vulnerabilities can combine.

My First Thought

One vulnerability alone may not look dangerous.

The Main Idea

Imagine two weak doors.

One lets someone enter. Another lets someone open a locker.

Together they create a bigger problem.

What I Tried

Observed how session cookies behaved.

What I Noticed

Sensitive information could be accessed.

Why I Changed My Thinking

I stopped treating XSS and authentication as separate problems.

Why It Worked

Weak cookie protection and another vulnerability worked together.

Impact

Could expose passwords or sessions.

Fix

Use HttpOnly and secure cookie settings.

What I Learned

Small flaws can combine into large attacks.
