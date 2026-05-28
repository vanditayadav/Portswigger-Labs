Tools Used: Burp Repeater

Goal

Find sensitive information hidden inside API responses.

My First Thought

The screen may not show everything returned by the server.

Main Idea

Sometimes websites send extra hidden data to browsers even though users cannot directly see it.

What I Tried

1) Captured profile request

2) Sent request to Repeater

3) Checked raw response

What I Noticed

Sensitive information like API keys appeared in the response.

Why I Changed My Thinking

I realized the frontend hides information visually, but the browser still receives it.

Why It Worked

The server returned complete user objects instead of only necessary fields.

Impact

Attackers may steal:

1) API keys

2) tokens

3) private information

Fix

1) Send only required data

2) Remove sensitive fields from responses

3) Filter data server-side

What I Learned

Hidden data is still exposed data.
