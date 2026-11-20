---
title: "Privacy and security"
description: "Where Steady keeps patients' information, who can see it, and how it's protected: one server per practice in South Africa, POPIA, two-step sign-in, access logs and signed updates."
lead: "Patients tell Steady how they're really doing. That only works if it stays between them and their psychologist. Here's how Steady is built to keep it that way."
---

## One server per practice, in South Africa

Steady isn't one big database of everyone's patients. Each practice has its own Steady server, hosted in South Africa, holding only that practice's information. It isn't copied to OpenWorks IT's own systems or to any cloud service abroad.

Under POPIA, **the practice** is the *responsible party*: it decides how its patients' information is used. **OpenWorks IT** is the *operator*: it runs the server on the practice's behalf, handles the information only on the practice's instructions, and keeps it secure and confidential. That's set out in an operator agreement, which the master psychologist signs in the app before anything else. Among other things, OpenWorks IT must tell the practice within 24 hours if the server's security is ever compromised.

## Who sees what

| Who | What they see |
|---|---|
| A patient | Only their own check-ins, answers and exercises. Not their scores, which go to their psychologist. |
| A psychologist | Only their own patients, and a patient a colleague has shared with them, for example while that colleague is away (read only; the patient can see who in the app). Every time they open a patient's information, it's written to an access log. |
| The master psychologist | Their own patients' information. For every patient, only whether their app is set up and connected. They manage staff accounts and the practice's updates, read the access log, and can carry out account deletions patients have asked for. |
| The practice administrator | Patients' names and whether each one's app is set up and connected, never what they shared. They send invites, reset passwords, stop accounts and read the access log. |
| OpenWorks IT | In the app, a support account that sees the practice's staff and the server, and nothing about patients, not even their names. It resets staff passwords and restores locked accounts. OpenWorks IT also runs the server, so it can technically reach it, as any hosting company can; it uses that access only to keep the server running and to fix problems. |

## Signing in

Psychologists and administrators sign in with a password and a code from an authenticator app, and only from devices they've linked: a new phone or browser is linked with a code emailed to them. On a phone, Steady locks itself and opens with the phone's own screen lock. Before anything sensitive, such as a password reset or an export, they confirm it's them again.

Patients sign in with a password they choose when they join, and can turn on **Lock Steady** so it asks for their phone's screen lock too.

Passwords are reset by people at the practice, never by an emailed link. When the practice resets a patient's password, the patient finishes it with a code emailed to them, so whoever reset it can't sign in as the patient.

## What leaves the server

- **Notifications** say "New notification" and nothing else: never a name, a score or a note, not even what kind of thing is new. iPhones get them through Apple, Android phones through Google. The app fetches the details over its own encrypted connection once you've signed in.
- **Emails** carry only codes and notices about a person's own account, never anything anyone shared.
- **No analytics, adverts or trackers** in the app or on this site.

## Keeping it running safely

- **Encrypted connections** (HTTPS) between the app and the server, always.
- **Encrypted backups** every night, encrypted before they're stored, kept in South Africa and deleted after 30 days.
- **Signed updates.** A practice's server installs a new version only if OpenWorks IT has signed it with its key, so nobody else can push code to it.
- **Automated tests** run on every change before it can be released, including checks that one patient or psychologist can't reach another's information.
- **Checked every six hours.** Each server checks its own security and privacy, and the results go to OpenWorks IT's view of every practice's server. That view shows versions, health and backups, and never anything about patients.
- **Watched at the door.** Each server counts what it turns away, such as scans, wrong passwords and requests for what isn't there. It also keeps tripwires that nobody at the practice ever touches, so whoever touches one is looking for a way in. OpenWorks IT is told at once.

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
