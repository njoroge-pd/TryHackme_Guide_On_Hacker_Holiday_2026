# walkthrough-Hacker-Holiday-Day-6
#OSINT Lab: Overheard at Breakfast

The lab gives one file, a Discord screenshot of two guests at the Byte Lotus resort. The goal is to find Lambo's profile on Gravatar.
In the chat, Ponzi asks Lambo for his social media handle. Lambo says he doesn't use social media anymore, but he used to have a free tool where he uploaded a profile and linked his other accounts. He thinks the name started with a G. He also gives his email: 'lambobytelotushotel@gmail.com.'

A profile and avatar service starting with G is 'Gravatar.'It identifies people by a hash of their email, so I hashed the address after lowercasing it.
We can check the email using Gravatar email checker here:
'https://gravatar.com/site/check'

Putting the hash in the URL opened his public profile, which had what the challenge asked for.
Even after wiping his accounts, Lambo's profile was still reachable because anyone with his email can compute the hash. The one-letter hint was enough to name the platform, and the email gave me the way in.

