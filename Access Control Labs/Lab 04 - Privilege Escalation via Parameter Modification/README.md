Tools Used: Burp Suite Repeater

Goal

Become an administrator by modifying hidden parameters.

My First Thought

Role changes should only be controlled by administrators.

Main Idea

Sometimes websites accidentally expose hidden settings inside requests.

Changing those settings may change permissions.

What I Tried

1) Captured account update request

2) Observed hidden values like:

   Admin=false

3) Changed it to:

   Admin=true

What I Noticed

The application accepted the modified value.

Why I Changed My Thinking

I stopped seeing hidden fields as “display-only” values and started treating them like controllable settings.

Why It Worked

The server trusted user-submitted role values without verifying permissions.

Impact

Normal users may become administrators.

Fix

1) Ignore unauthorized fields

2) Allow only approved parameters

3) Control permissions server-side

What I Learned

Hidden fields are still controlled by users.
