---
title: 'Nota Hastag but a Hash'
description: 'Understanding Hashing'
pubDate: 'June 2, 2025'
heroImage: '/hash.png'
---

Have you ever thought about what happens to your password when you sign up for a website? You probably type something like “password123” and hit submit, but that password doesn’t get stored as you wrote it, insted the site uses something called password hashing. Basically, hashing is like putting your password through a scrambler that turns it into random letters and numbers, and once it’s jumbled up, there’s no easy way to put it back to "password123” so even if someone manages to get into the database, they only see that scrambled string, not your actual password.

When you create an account, the website takes your password, runs it through a hashing algorithm you might’ve heard of, bcrypt, Argon2, or SHA-256, and saves only the final hash. Later, when you log in, the site takes the password you enter, hashes it again, and checks if it matches the stored hash. If they match, you’re good to go. Kinda like compairing two pieces of a puzzles that should look identical.

Theres more to hashing though! Websites often add something called a “salt” before hashing. Salt is a random string that gets mixed into your password before it randomises it. That way, if two people accidentally pick the same password like “password123,” their hashes will still look different, and this extra step makes it way harder for hackers who try to crack passwords using pre-made tables of common hashes.

Password hashing, especially with a salt, is a important security step, and while it doesn’t make you completly secure, and while hackers are always trying new tricks, it’s one of the best ways to keep your password safe. Next time you sign up for something, you can remember hashing!








