# Ethiopia : Guitar Strings
**Category:** Reverse Engineering
**Points:** 100
**Bonus:** 30


## Problem

You have been given a binary file by the DPR the file contains the key to unlock the refinery Download [WIN] [OSX] [LINUX]

**Hint:** quit stringing me along
**File:** quit-stringing-me-along.app, quit-stringing-me-along.elf, quit-stringing-me-along.exe


## Solution

Open any of the files using a text editor (I used TextEdit)

By searching NSC, we found the string below

```
TlNDe2ZsYWdfaXNfbGFra2FfdGhpc19sYWtrYV90aGF0fQ==
```

This is definitely base64 encoded, decoded this and got

```
NSC{flag_is_lakka_this_lakka_that}
```

Hence, the flag is **NSC{flag_is_lakka_this_lakka_that}**.