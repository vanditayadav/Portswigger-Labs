Tools Used: Browser, Burp Suite

Goal

Access private files by changing file numbers.

My First Thought

Downloaded files should only belong to the correct user.

Main Idea

Predictable file names create predictable access paths.

What I Tried

1) Downloaded transcript file

2) Changed:

   9.txt

   to

   1.txt

What I Noticed

Other users’ files became accessible.

Why It Worked

The server never checked ownership before serving files.

Impact

Private conversations and sensitive records may leak.

Fix

1) Verify file ownership

2) Use random filenames

3) Protect static downloads

What I Learned

Static files also need access control.
