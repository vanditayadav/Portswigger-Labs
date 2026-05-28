Tools Used: Burp Repeater

Goal

Bypass access control using forged Referer headers.

My First Thought

Headers coming from users should never be trusted for security decisions.

Main Idea

The browser sends many headers automatically, but users can still modify them.

What I Tried

1) Added fake Referer header

2) Pointed it to admin page

What I Noticed

The request became authorized.

Why It Worked

The server trusted the Referer value instead of checking the actual user role.

Impact

Attackers may bypass authorization using fake request headers.

Fix

1) Ignore client-controlled headers for authorization

2) Validate roles server-side

3) Trust sessions, not headers

What I Learned

Anything coming from the client can be modified.
