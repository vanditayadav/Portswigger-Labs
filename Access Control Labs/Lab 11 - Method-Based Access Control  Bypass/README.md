Tools Used: Burp Repeater

Goal

Bypass restrictions by changing HTTP methods.

My First Thought

Access control should protect the feature itself, not just one request type.

Main Idea

Sometimes websites secure POST requests but forget GET requests.

What I Tried

1) Changed:

   POST

   to

   GET

What I Noticed

The restricted action still worked.

Why It Worked

The server protected only one request method.

Impact

Attackers may bypass restrictions and perform admin actions.

Fix

1) Protect all methods equally

2) Reject unexpected methods

3) Apply global authorization checks

What I Learned

Changing small request details can bypass weak protections.
