# Iran : Caesars Laravel
**Category:** Web Application
**Points:** 50
**Bonus:** 5

    
## Problem

Well, God save the King.

**Hint:** is laravel in production secure?
**Link:** http://ec2-18-219-23-67.us-east-2.compute.amazonaws.com:9090


## Solution
The link given was to a web app.

And from the hint, `is laravel in production secure?`, absolutely no!

There's been a recent trend about a laravel vulnerability whereby if misoconfigured, navgating to the file `/.env` discloses the server configurations

Then, accessing this endpoint on the link given, 

```
http://ec2-18-219-23-67.us-east-2.compute.amazonaws.com:9090/.env
```

Found the hash below

```
uzj{shyhcls_pm_tpzjvumpnbylk_pz_cbsulyhisl}
```

Decoded using Caesar Cipher as stated in the problem title to
 
```
NSC{laravel_if_misconfigured_is_vulnerable}
```

Hence, the flag is **NSC{laravel_if_misconfigured_is_vulnerable}**.