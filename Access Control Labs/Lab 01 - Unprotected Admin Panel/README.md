Tools Used: Web Browser

Goal

Find an admin panel that was not properly protected.

My First Thought

I thought an admin panel should always ask for admin login or special permissions before opening.

Main Idea

Sometimes websites try to “hide” admin pages instead of actually protecting them.

It is similar to hiding an important room behind a normal-looking door without locking it.

What I Tried

1) Explored the website URLs

2) Tried common admin paths manually

3) Tested paths like /admin or /administrator-panel

What I Noticed

One of the guessed paths opened the admin panel directly.

No permission checks were stopping access.

Why I Changed My Thinking

At first I thought I would need special credentials.

Then I realized the website was only depending on the URL being unknown.

Why It Worked

The server never checked whether the user was actually an administrator.

It only checked whether the correct path was requested.

Impact

Anyone who discovers the admin URL can access sensitive features.

This may allow:

1) deleting users

2) changing settings

3) controlling the application

Fix

1) Always verify user roles on the server side

2) Restrict admin features to authorized users only

3) Never depend on hidden URLs for security

What I Learned

Hiding something is not the same as protecting it.
