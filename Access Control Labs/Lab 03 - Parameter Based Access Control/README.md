Tools Used: Burp Suite Proxy, Repeater

Goal

Access another user’s account by changing URL parameters.

My First Thought

The website should only allow users to access their own account information.

Main Idea

If a website trusts user-controlled parameters too much, changing those parameters may change account access.

What I Tried

1) Logged into my own account

2) Observed:

   /my-account?id=wiener

3) Changed:

    id=wiener

4) to

    id=admin

What I Noticed

The website loaded another user’s account.

Why I Changed My Thinking

I realized the website trusted the URL parameter more than the logged-in session.

Why It Worked

The server used the parameter value directly without checking ownership.

Impact

Attackers may access:

1) private accounts

2) personal information

3) admin features

Fix

1) Use server-side session identity

2) Verify ownership before showing data

3) Never trust user-controlled identifiers directly

What I Learned

Changing a small parameter can completely change access boundaries.
