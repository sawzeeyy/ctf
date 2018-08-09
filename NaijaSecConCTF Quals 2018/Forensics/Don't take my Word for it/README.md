# Austria : Don't take my Word for it
**Category:** Forensics
**Points:** 90


## Problem

The fraudulent fuel marketer thought he was too smart with their empty files but you have been engaged by NNPC to prove them otherwise.

**Hint:** no
**File:** flaggy.rar


## Solution
The file given above is a rar file. Extracted this and got 2 more files

```
- flag.rar
- keys.docx
```

Then had no luck opening **keys.docx** and **flag.rar** requires a password.

Afterwards, I opted to view **keys.docx** using a *text editor*, I used text edit and got the information below:

```
The key you seek is youreallywanttobecomethebestright?
```

Then used this key, *youreallywanttobecomethebestright?* to extract the contents of **flag.rar**. Then we got one more file, **flag.txt** which contains the following:

```
The flag you seek is NSC{paSSW0rd_nOT_H1dD3N}
```

Hence, the flag is **NSC{paSSW0rd_nOT_H1dD3N}**.

![Screen caption](assets/path-to-screen.png)