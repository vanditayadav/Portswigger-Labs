Goal

Test whether password change functionality leaks information.

My First Thought

Most protections focus only on login pages.

The Main Idea

Sometimes side doors are weaker than the main entrance.

What I Tried

Observed behavior while testing password changes.

What I Noticed

Error messages changed depending on input.

Why I Changed My Thinking

I realized internal features may reveal hidden clues.

Why It Worked

The application accidentally revealed information through validation.

Impact

Can help attackers guess passwords.

Fix

Use identical responses.

What I Learned

Internal pages need security too.
