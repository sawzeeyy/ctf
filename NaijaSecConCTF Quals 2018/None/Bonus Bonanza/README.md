# Brazil : Bonus Bonanza
**Category:** None, Quiz
**Points:** 100
**Bonus:** 5


## Problem

Dear Gamers,

We are glad you're able to join us for this year's #NaijaSecConCTF

We however seem to have a major challenge at hand. The theme for this year’s games is centered on the Fuel Scarcity. For a while now, we've encountered recurring and lingering fuel scarcity. Our insistence on the Directorate for Petroleum Resources (DPR) to stem this tide is not yielding any positive result.

At NaijaSecCon, we sincerely recognize the need to have solution providers like your good-selves to create a leeway for others to tread on. That is why your skills and tactics are required towards resolving this painful recurring fuel-scarcity menace.

The last time we checked, the offices of the DPR officers were locked. The key to unlocking the door that leads to land of oil bounty for the nation is faulty. You and your team have been given this simple task of gaining entrance into the office to claim the bounty for yourselves and the nation at large.

Alas! We found the faulty key. But you and your team have to fix it before you can gain entrance.

V2VsY29tZS4gSWYge W91IGFyZSByZWFkaW5nIHRoaXMgdGhlbiBpdCBtZWFucyB0

aGF0IHlvdSBhcmUgb2?5lIG9mIHRoZSBlbGl0ZSBrZXkgZml4ZXJzLiBZZXMsIHlv

dSBoYXZlIGFjY2VzcywgYnV0IGRpZCB5b3UgdGhpbmsga2?hha2kgZXF1YXRlcyBs

ZWF0aGVyPw0KTGV0IHlvdXIgdGVhbSBub3cgcHJvdmUgdGhhdCB0aGV5IGFyZSB3

b3J0aHkgYW5kIHlldCBnbyBhaGVhZCB0byBmaXggdGhlIHJlbWFpbmluZ?yBwYXJ0

IG9mIHRoaXMga2V5LCB0byBqb2?luIHRoZSBoYWxsIG9mIGZhbWUgb2YgY3J5cHRv

LWtpbmdzLg0KUHJvdmUgYW5kIGxldCdzIHNlZ?SBpZiB5b3UgYXJlIHdvcnRoeS4u

LgpUaGUgYm9udXMgZmxhZyB?5b3Ugc2VlayBpcyBWR3hPUkdVemJGQldXRW9nWmxs

dGJFaFlNRWwzWW14V1Z HWlJQVDA9Cg==

 

We know you can fix this key and get handsomely REWARDED for your efforts. 

That is why we are pleased that you are in this game to PLAY WITH THE REST AND BECOME THE BEST.



Happy gaming!


## Solution
Mere looking at this, it looks like a base64 encoded string
```
V2VsY29tZS4gSWYge W91IGFyZSByZWFkaW5nIHRoaXMgdGhlbiBpdCBtZWFucyB0

aGF0IHlvdSBhcmUgb2?5lIG9mIHRoZSBlbGl0ZSBrZXkgZml4ZXJzLiBZZXMsIHlv

dSBoYXZlIGFjY2VzcywgYnV0IGRpZCB5b3UgdGhpbmsga2?hha2kgZXF1YXRlcyBs

ZWF0aGVyPw0KTGV0IHlvdXIgdGVhbSBub3cgcHJvdmUgdGhhdCB0aGV5IGFyZSB3

b3J0aHkgYW5kIHlldCBnbyBhaGVhZCB0byBmaXggdGhlIHJlbWFpbmluZ?yBwYXJ0

IG9mIHRoaXMga2V5LCB0byBqb2?luIHRoZSBoYWxsIG9mIGZhbWUgb2YgY3J5cHRv

LWtpbmdzLg0KUHJvdmUgYW5kIGxldCdzIHNlZ?SBpZiB5b3UgYXJlIHdvcnRoeS4u

LgpUaGUgYm9udXMgZmxhZyB?5b3Ugc2VlayBpcyBWR3hPUkdVemJGQldXRW9nWmxs

dGJFaFlNRWwzWW14V1Z HWlJQVDA9Cg==`
```

Then, it was base64 decoded to 

```
Welcome. If you are reading this then it means that you are one of the elite key fixers. Yes, you have access, but did you think khaki equates leather?
Let your team now prove that they are worthy and yet go ahead to fix the remaining part of this key, to join the hall of fame of crypto-kings.
Prove and let's see if you are worthy...
The bonus flag you seek is VGxORGUzbFBWWEogZlltbEhYMEl3YmxWVGZRPT0=
```

And like wise the bonus flag was base64 decoded to

```
TlNDe3lPVXJ fYmlHX0IwblVTfQ==
```

And finally, the string above which look no more than a base64 encoded string was decoded to:

```
NSC{yOUr_biG_B0nUS}
```

Hence the flag is **NSC{yOUr_biG_B0nUS}**.