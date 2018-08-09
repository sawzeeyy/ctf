# Oman : PolyCipher
**Category:** Cryptography
**Points:** 70


## Problem

The Police Inspector, before he was handed off the DPR case, could only transfer this document to the IPO. Help the IPO further his case by explaining what the Inspector meant.\n\nEnclose flag in NSC{_ _}

**Hint:** no
**File:** polythenebius.txt


## Solution

This was a relatively easy solve using the table at https://en.wikipedia.org/wiki/Polybius_square

Then I coded a script to speed the process:

```
#!/usr/bin/env python3
# PolyCipher - NaijaSecCon
alphabets = [['A', 'B', 'C', 'D', 'E'], ['F', 'G', 'H', 'I', 'K'], ['L', 'M', 'N', 'O', 'P'], ['Q', 'R', 'S', 'T', 'U'], ['V', 'W', 'X', 'Y', 'Z']]
output = ''
with open('polythenebius.txt') as text:
    for texts in text:
        texts = texts.strip()
        output += alphabets[int(texts[0]) - 1][int(texts[1]) - 1]
print(output)
```

Running the script gave the following output
```
FUELSCARCITYNOGOOD
```

Hence, the flag is **NSC{fuel_scarcity_no_good}**.