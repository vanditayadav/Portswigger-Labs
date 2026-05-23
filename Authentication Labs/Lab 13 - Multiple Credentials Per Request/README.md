Goal

Test whether one request can contain many login attempts.

My First Thought

One request should equal one attempt.

The Main Idea

Imagine a guard allows one person through a gate at a time.

Someone arrives carrying a bus full of people.

The guard only counts one vehicle.

What I Tried

Observed how request data was processed.

What I Noticed

The application accepted unexpected formats.

Why I Changed My Thinking

I shifted focus from request count to request content.

Why It Worked

Input handling allowed multiple attempts together.

Impact

Rate limiting becomes weaker.

Fix

Validate input structure carefully.

What I Learned

Unexpected formats create unexpected problems.
