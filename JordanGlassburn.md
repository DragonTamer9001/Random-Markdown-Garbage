
In my early ages of coding, such as in Computer Science 1, I had many of these CWEs, but none plagued me more than one.
Out-of-bounds Read. One of my greatest adversaries, and grade deducters. 
In short, out of bounds reading is when the program attempts to read data that doesn't exist.
This causes huge issues, such as crashing, or potentially opening up a way for outside parties to put unwanted data into the program.
While in my past I had this issue quite frequently, I have luckily learned how to fix this.

Fixing the out-of-bounds read is quite simple.
When implementing something that reads data, be sure to include a safeguard so that reading out-of-bounds cannot happen under any circumstances.
For example, if you are reading an array with a for loop, you must make sure to set the "i" variable to not go out of bounds of the array. 
A more famous example of out-of-bound reading is the "Heartbleed bug", effecting OpenSSL 1.0.1. 
This happens when the program reads "Heartbeat Extension" packets, which can cause an out-of-bounds read, which, of course, provides a way for outside parties to exploit this.

When I finally had to start learning how to fix the out-of-bounds reads for my programs, it made me realize how many of them I truly had in my previous projects.
So many potential issues, so many backdoors that outside sources could use.
I'd like to think that nowadays I am better about letting potential CWE's get in my code, although I'm sure that there are some that are passing right over my head every time.
Looking into these CWE's have made me think back on code I've written and submitted for grading, thinking how I could have made them more secure, more safe.
But one things for certain: I've learned my lesson for out-of-bounds reads, and hopefully people will continue to prevent this easily over-seen issue from causing security problems.
