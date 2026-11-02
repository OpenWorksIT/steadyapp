---
title: "Privacy and security"
description: "Where Steady keeps patients' information, who can see it, and how it's protected: one server per practice in South Africa, POPIA, two-step sign-in, access logs and signed updates."
lead: "Patients tell Steady how they're really doing. That only works if it stays between them and their psychologist. Here's how Steady is built to keep it that way."
---

## One server per practice, in South Africa

Steady isn't one big database of everyone's patients. Each practice has its own Steady server, hosted in South Africa, holding only that practice's information. It isn't copied to OpenWorks IT's own systems or to any cloud service abroad.

Under POPIA, **the practice** is the *responsible party*: it decides how its patients' information is used. **OpenWorks IT** is the *operator*: it runs the server on the practice's behalf, handles the information only on the practice's instructions, and keeps it secure and confidential.

## Who sees what

| Who | What they see |
|---|---|
| A patient | Only their own check-ins, answers and exercises. Not their scores, which go to their psychologist. |
| A psychologist | Only their own patients. Every time they open a patient's information, it's written to an access log. |
| The master psychologist | Their own patients, plus the practice's settings and updates. They can carry out account deletions patients have asked for. |
| OpenWorks IT | Runs the server, so it can technically reach it, as any hosting company can. It uses that access only to keep the server running and to fix problems. |

## Signing in

Psychologists and administrators sign in with a password and a code, and only from devices they've linked. Patients sign in with a password they choose when they join.

## What leaves the server

- **Notifications** say only that there's something new. They never carry a name, a score or a note. The app fetches the details over its own encrypted connection once you've signed in.
- **Android notifications** don't go through Google by default.
- **No analytics, adverts or trackers** in the app or on this site.

## Keeping it running safely

- **Encrypted connections** (HTTPS) between the app and the server, always.
- **Encrypted backups** every night, encrypted before they're stored.
- **Signed updates.** A practice's server installs a new version only if OpenWorks IT has signed it with its key, so nobody else can push code to it.
- **Automated tests** run on every change before it can be released, including checks that one patient or psychologist can't reach another's information.

## Open source

Steady is free and open-source software under the GNU AGPL. Anyone can [read the code](https://github.com/OpenWorksIT/steady), check how it handles information, and run it themselves. There's no hidden part.

## Not an emergency service

Steady doesn't watch patients around the clock, and its flags are review aids for the psychologist, not alarms. Every patient screen says so and shows crisis numbers: SADAG on 0800 567 567, or 112 from a mobile phone.

## Deleting an account

A patient can ask to delete their account in the app. Their practice carries it out within 30 days, after copying what the law requires it to keep in the clinical file (HPCSA Booklet 9). [How it works](/patients/#delete).

## Privacy policy

The full [Steady privacy policy](https://www.openworks.co.za/steady/privacy/) sets out what's collected, why, for how long, and patients' rights under POPIA.

## Report a security problem {#report}

If you think you've found a security problem in Steady, email [info@openworks.co.za](mailto:info@openworks.co.za) before telling anyone else, with enough detail for us to reproduce it. We'll reply, keep you posted, and credit you if you'd like.
