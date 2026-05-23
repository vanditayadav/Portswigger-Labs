Goal

Check whether OTP verification correctly stays linked to the right user.

My First Thought

I assumed OTP codes should always stay connected to one user account.

The Main Idea

Imagine a school gives roll numbers for an exam, but students can freely change the roll number written on their sheet.

That would create confusion.

What I Tried

Observed how the website tracked identity during OTP verification.

What I Noticed

Some values controlling identity looked editable.

Why I Changed My Thinking

Instead of focusing on the OTP itself, I focused on how the application remembered users.

Why It Worked

The website relied too much on user-controlled information.

Impact

May allow access to another account.

Fix

Store identity only on server-side sessions.

What I Learned

Identity should never be controlled by users.
