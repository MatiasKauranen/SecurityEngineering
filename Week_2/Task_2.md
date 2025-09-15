# Task 2: Cards and Payments
## Why do modern payment cards use a chip and not a magnetic stripe?
Most important reason is improved security. Magnetic cards are easier to copy and relied on signature verification which could be easily exploited. Chips on other hand are much harder to copy and they also have pin code verification which is much better.
## What are EMV Certificates and why are they relevant for payment protection?
They are way to verify valid payment cards. These validations are  issued by EMV Certificate Authority. EMV Certificates makes paying with payment cards more secure.
## What attacks exist against payment cards?
**Card-not-present**: Mail order fraud, since only information on card is required to use the card and not physical card itself criminals can for example order something from internet with stolen card information.

**Contactless payment**: PIN bypass attack, criminals can use vulnerabilities to bypass PIN code input when using stolen card.
## How is multi-factor authentication (MFA) used in banking?
MFA especially in banking relies on multiple sources for verification before accessing banking services. Many banks including my use account number (something you know) and phone verification (something you have).
## How does multi-factor authentication increase payment security?
Its much less likely that criminals gets multiple source of authentication instead of just one.
## What MFA methods are you using in you daily life?
Phone authentication for example Microsoft Authenticator. I also use email authentication for several services.
## What attacks exists against different forms of 2FA? 
**Time-based-one-time-password:** One time passwords must be be input on seperate page which means they can be phished by creating fake website for example to receive correct authentication number, however the number is valid only for brief moment which makes this attack very hard to manage.  
**Text Message:** Fatigue attack, user is spammed by large volume of authentication requests in hopes that they accept atleast once.