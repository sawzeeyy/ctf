# Turkey : The Head Boy
**Category:** Forensics
**Points:** 100


## Problem

The DPR just published a memo with this in it...\"For any issue, ensure you report to the HEAD of Department or else you get punished.\" I have been trying to view it on my system since yesterday. Help me please.

**Hint:** no
**File:** headboy.pdf


## Solution
An invalid PDF file was given and viewing the raw file showed that the file was an image as it had `PNG` header. The challenge title was the clue afterall.


Renamed the file to `headboy.png`, and still no success.

Then comparing the file with other PNG files shows that some chunks were missing.

Added these chunks and got the image with the flag
```
NSC{hEAdeR5_ArE_m@g1CaL}
```

Hence, the flag is **NSC{hEAdeR5_ArE_m@g1CaL}**.