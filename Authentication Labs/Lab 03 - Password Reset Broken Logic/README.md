Goal

Check whether reset tokens truly belong to users.

My First Thought

Password reset links should only work for their owner.

The Main Idea

Imagine someone receives a movie ticket.

The security guard checks:

"Is this a real ticket?"

But forgets:

"Does this ticket belong to this person?"

What I Tried

Observed reset requests and changed parameters.

What I Noticed

Token checking existed but ownership checking looked weak.

Why I Changed My Thinking

I focused less on whether token existed and more on who owned it.

Why It Worked

The website checked token validity but not ownership properly.

Impact

Can lead to account takeover.

Fix

Bind tokens to users strongly.

What I Learned

Correct values alone are not enough. Relationships matter too.
