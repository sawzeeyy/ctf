# Mexico : Its not as easy or as difficult as you think
**Category:** Cryptography
**Points:** 200


## Problem

I wonder what  this string is hiding \"VGhlIHRva2VuIHlvdSBzZWVrIGlzIHdlbG9kcnVuZg==

**Hint:** Try harder
**File:** no


## Solution
The lucky guess for this is that it's a base64 encoded string, 

```
VGhlIHRva2VuIHlvdSBzZWVrIGlzIHdlbG9kcnVuZg==
```
which was then decoded to 

```
The token you seek is welodrunf
```

The token / flag is definitely scrambled, using a web service, https://wordunscrambler.me/unscramble, and passing the scrambled data as the input, we got the string below:
```
wonderful
```
This was indeed wonderful!

Hence , the flag is **NSC{wonderful}**.
