Tools Used: Burp Repeater

Goal

Bypass frontend restrictions using custom headers.

My First Thought

Different layers of the website may interpret requests differently.

Main Idea

If frontend and backend systems disagree about request paths, attackers may exploit the confusion.

What I Tried

1) Requested blocked admin page

2) Added:

   X-Original-URL: /admin

What I Noticed

The backend processed the hidden path.

Why It Worked

Frontend checked one path while backend trusted another.

Impact

Attackers may bypass frontend restrictions completely.

Fix

1) Ignore override headers

2) Apply same checks everywhere

3) Standardize request handling

What I Learned

Security gaps often appear between different system layers.
