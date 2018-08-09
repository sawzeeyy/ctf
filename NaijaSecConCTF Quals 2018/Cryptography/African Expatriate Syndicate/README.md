# Uzbekistan : African Expatriate Syndicate
**Category:** Cryptography
**Points:** 200


## Problem

256 foreign suspects have been arrested by the Nigeria Immigration Service, thanks to DPR. One of them was caught with this document he said was got at the \"naijasecconctf\", which is assumed to be Top Secret.

**Hint:** no
**File:** soso.aes


## Solution
A salted file was given and after a few searches, we finally got this link, https://www.shellhacks.com/encrypt-decrypt-file-password-openssl/, which explained all we needed to obtain the flag.


```
> openssl enc -aes-256-cbc -d -in file.txt.enc -out file.txt -k PASS

> openssl enc -aes-256-cbc -d -in soso.aes -out secretfile.txt -k naijasecconcctf
```
Running the commands above, we got the flag 

```
NSC{aEs_i5_sTroNG}
```

Hence, the flag is **NSC{aEs_i5_sTroNG}**.