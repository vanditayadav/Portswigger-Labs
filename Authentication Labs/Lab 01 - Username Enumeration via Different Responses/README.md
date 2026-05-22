Tools Used: Burp Suite Intruder

Goal

Find out whether the website accidentally reveals if a username exists.

My First Thought

I thought every failed login should show exactly the same message.

For example:

"Invalid username or password"

A secure application should not tell us whether the username exists.

The Main Idea

Imagine knocking on apartment doors.

Door 1 says: "Nobody lives here."

Door 2 says: "Wrong key."

Now I already know someone lives behind Door 2.

The same thing happens with websites.

What I Tried
Intercepted login request
Sent request to Intruder
Tried multiple usernames
Kept password same
Compared responses
What I Noticed

Most responses looked similar.

But one response had a different length and behavior.

That small difference became a clue.

Why I Changed My Thinking

Initially I focused on passwords.

Then I realized the username itself was leaking information.

Why It Worked

The website handled real users and fake users differently.

Impact

Attackers can find valid users before attacking passwords.

Fix

Always return identical error messages.

What I Learned

Tiny differences sometimes reveal huge problems.
