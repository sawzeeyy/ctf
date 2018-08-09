# Portugal : Numbers are magical
**Category:** Cryptography
**Points:** 90


## Problem

An agent has been missing for weeks and the password to the secure vault is required to proceed with his primary mission. All you have right now is a text file you found on his pen drive. Can you find any clues\n\nEnclose flag in NSC{}

**File:** Wired.txt 


## Solution

A text file was given.

And as it appears, there's a lot of text in there, then I noticed there were a few numbers. 

Extracted the numbers in the text in the order they appear and got the flag

```
#!/usr/bin/env python3
# Magical Numbers - NaijaSecCon

fh = open('magical.txt').readlines()
fh = [j for i in fh for j in i]
output = ''
for i in fh:
    try:
        num = int(i)
        output += i
    except: continue
print('The flag is NSC{}{}{}'.format('{',output,'}'))
```
Running the script above gave the following output:

```
The flag is NSC{4263}
```

Hence, the flag is **The flag is NSC{4263}**.