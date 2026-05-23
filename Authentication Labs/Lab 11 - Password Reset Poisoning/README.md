Goal

Check whether password reset links trust user input.

My First Thought

Password reset links should always come from trusted sources.

The Main Idea

Imagine a delivery company asks customers:

"Which address should we deliver to?"

and trusts whatever is written.

That can become dangerous.

What I Tried

Observed how reset links were created.

What I Noticed

The website trusted information coming from requests.

Why I Changed My Thinking

I focused less on reset tokens and more on where links were generated.

Why It Worked

The application trusted external routing information.

Impact

Reset links may be redirected toward attackers.

Fix

Use trusted server-side domains only.

What I Learned

Even supporting information can become dangerous.
