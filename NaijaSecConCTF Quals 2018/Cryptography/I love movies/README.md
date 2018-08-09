# Italy : I love movies
**Category:** Cryptography
**Points:** 40


## Problem

lvkmu zkxdrob: vyxq vsfo ___ ____\n\n\nEnclose flag in NSC{_}

**File:**  

**Hint:** The commandments

## Solution

This was the first challenge after the bonus challenge released few days before the CTF.

Mere looking at this, they seem to be a ROT sequence. And feeding this input to a ROT decoder, 
 
 
```
http://theblob.org/rot.cgi?text=lvkmu zkxdrob: vyxq vsfo ___ ____

```
It was seen that the right decoding was on ROT 16

```
black panther: long live ___ ____
```

Googling this, we found the popular / trending movie title,

```
Black Panther: Long Live The King
```

From the problem description, we were to enclose flag in the format `NSC{}`

Hence, the flag is **NSC{the_king}**.