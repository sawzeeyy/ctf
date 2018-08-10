# Zimbabwe : Book Me On
**Category:** Cryptography
**Points:** 150


## Problem

The manager of ASDF Oil is secretly a cryptographer but he never knew the DPR has a crop of great guys who would unravel the secret he embedded in this file. You are one of the great guys...\n\nEnclose flag in NSC{_ _}

**Hint:** no
**File:** How_Smartcard-Payment-Systems-Fail.pdf  


## Solution
A PDF file was given for this challenge and as it looks, this was a presentation presented at **Black Hat 2014**.

The first thing that came to mind was to find the original file and compare these files.

Got the file and at first, the difference wasn't visible until we had to view the file as a text (raw view of file) and saw that some numbers were appended after the *EOF* (End of File) which is't in the original file.

Below is the numbers:

```
2, 6, 2


10, 3, 3


24, 9, 1


1, 1, 1


5, 1, 1


8, 2, 1


10, 5, 1


8, 7, 1


8, 11, 1


2, 1, 2


34, 10, 2


32, 8, 8


5, 6, 1


6, 5, 2


6, 3, 1


13, 1, 2


18, 10, 4


18, 12, 2
```


Proceeding further, we didn't know what to do with this but later got to know that these numbers were references to **page, line, and word** numbers respsectively. Then we derived the following result


```
2, 6, 2 = Canada 

10, 3, 3 = it  

24, 9, 1 = precompute

1, 1, 1 = How

5, 1, 1 = EMV

8, 2, 1 = Replace

10, 5, 1 = So

8, 7, 1 = Use

8, 11, 1 = selling

2, 1, 2 = EMV

34, 10, 2 = book

32, 8, 8 = or

5, 6, 1 = off

6, 5, 2 = key

6, 3, 1 = security

13, 1, 2 = tamper

18, 10, 4 = Omar

18, 12, 2 = only
```

Taking a keen look at results above, one could see these are random words and some are even repeated. The challenge here is to convert these words to a flag: these were the first letter of each words.
 
```
CipHERSUsEbookstOo
```

Pronounced: *Ciphers Use Books Too*

Hence, the flag is **NSC{CipHERS_UsE_books_tOo}**.