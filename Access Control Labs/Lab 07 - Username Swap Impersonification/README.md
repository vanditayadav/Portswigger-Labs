Tools Used: Burp Repeater

Goal

Perform actions on another user’s account.

My First Thought

The session should define who performs an action.

Main Idea

If a website trusts usernames inside forms more than sessions, changing the username changes the target account.

What I Tried

1) Captured profile update request

2) Changed:

   username=wiener

   to

   username=carlos

What I Noticed

The action applied to another account.

Why It Worked

The server trusted the submitted username value directly.

Impact

Attackers may modify:

1) profiles

2) settings

3) passwords

Fix

1) Use session identity only

2) Validate ownership before changes

What I Learned

Identity should come from the session, not from editable form values.
