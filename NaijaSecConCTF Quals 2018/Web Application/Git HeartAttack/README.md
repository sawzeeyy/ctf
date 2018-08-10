# China : Git HeartAttack
**Category:** Web Application
**Points:** 75
**Bonus:** 5


## Problem

I made a terrible mistake. I ignored instructions. Help me before someone sees this and causes me a heart attack.

**Hint:** how do I avoid pushing secrets to git
**Link:** http://ec2-18-219-23-67.us-east-2.compute.amazonaws.com:9191



## Solution

The link given was to a web app. 

Deducing from the hint, its talking about how one could prevent pushing some files to git. This was an easy one and like anyone would have thought, using the `.gitignore` helps very much to define directories  / files that you do not want to be committed when you push to github.

Then, appending the URL with `./gitingore`, i.e http://ec2-18-219-23-67.us-east-2.compute.amazonaws.com:9191/.gitignore contained so many texts and within is an encoded string

```
4E53437B7573655F6769745F776973656C795F746F5F61766F69645F73746F726965735F746861745F746F7563687D
```

Easy solve! Decoded this ASCII hex to 
```
NSC{use_git_wisely_to_avoid_stories_that_touch}
```

Hence, the flag is **NSC{use_git_wisely_to_avoid_stories_that_touch}**.