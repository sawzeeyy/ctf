# Central African Republic : DocuConnect
**Category:** Forensics
**Points:** 90


## Problem

NNPC hijacked this document from the network of a suspected marketer. Help them discover what they were sharing with others.

**Hint:** flag is not all in small letters
**File:** TheFlag.doc


## Solution

A word document file was given

Two links to `www.naijaseccon.com` was found in the document

```
https://www.linkedin.com/company/naijaseccon-cybersecurity-conference/redirect?url=http%3A%2F%2Fwww%2Enaijaseccon%2Ecom&urlhash=ojGk&actionToken=p%3Dp%253Dbiz-company-login%2526c%253D23632a14-5702-454f-99f0-001e62aa616c%2526m%253Dcompany_feed%2526n%253D0%26t%3Da%253DisFolloweeOfPoster%25253Dfalse%252526distanceFromActor%25253D-1%252526actorType%25253D%252526likedByUser%25253Dfalse%252526targetId%25253D%252526recentCommentUrns%25253D%252526targetType%25253D%252526sponsoredFlag%25253DORGANIC%252526verbType%25253Dlinkedin%2525253Ashare%252526objectType%25253Dlinkedin%2525253Acontent%252526totalShares%25253D0%252526activityId%25253Durn%2525253Ali%2525253Aactivity%2525253A6262886658392223744%252526recentLikerUrns%25253D%252526actorId%25253Durn%2525253Ali%2525253Acompany%2525253A13268905%252526totalComments%25253D0%252526relevanceScore%25253D0%2E0%252526recentCommenterUrns%25253D%252526isPublic%25253Dtrue%252526time%25253D-1%252526totalLikes%25253D0%252526objectId%25253Durn%2525253Ali%2525253Acontent%2525253AJPEG%2525252FIMG%2525252F6b7dfed041e04549b2c5fd6b2327878e%252526distanceFromNestedActor%25253D-1%2526s%253DORGANIC%2526u%253Durn%25253Ali%25253Aactivity%25253A6262886658392223744&atv=2&actionType=CLICK
```


```
https://www.linkedin.com/company/naijaseccon-cybersecurity-conference/redirect?|theflag.dochttp://the-flag-you-seek-is-NSC%7bHttP_will_mAkE_yoU_loST%7d\/url=http%3A%2F%2Fwww%2Enaijaseccon%2Ecom&urlhash=ojGk&actionToken=p%3Dp%253Dbiz-company-login%2526c%253D23632a14-5702-454f-99f0-001e62aa616c%2526m%253Dcompany_feed%2526n%253D0%26t%3Da%253DisFolloweeOfPoster%25253Dfalse%252526distanceFromActor%25253D-1%252526actorType%25253D%252526likedByUser%25253Dfalse%252526targetId%25253D%252526recentCommentUrns%25253D%252526targetType%25253D%252526sponsoredFlag%25253DORGANIC%252526verbType%25253Dlinkedin%2525253Ashare%252526objectType%25253Dlinkedin%2525253Acontent%252526totalShares%25253D0%252526activityId%25253Durn%2525253Ali%2525253Aactivity%2525253A6262886658392223744%252526recentLikerUrns%25253D%252526actorId%25253Durn%2525253Ali%2525253Acompany%2525253A13268905%252526totalComments%25253D0%252526relevanceScore%25253D0%2E0%252526recentCommenterUrns%25253D%252526isPublic%25253Dtrue%252526time%25253D-1%252526totalLikes%25253D0%252526objectId%25253Durn%2525253Ali%2525253Acontent%2525253AJPEG%2525252FIMG%2525252F6b7dfed041e04549b2c5fd6b2327878e%252526distanceFromNestedActor%25253D-1%2526s%253DORGANIC%2526u%253Durn%25253Ali%25253Aactivity%25253A6262886658392223744&atv=2&actionType=CLICK
```

URL decoding the second link gives

```
https://www.linkedin.com/company/naijaseccon-cybersecurity-conference/redirect?|theflag.dochttp://the-flag-you-seek-is-NSC{HttP_will_mAkE_yoU_loST}\/url=http://www.naijaseccon.com&urlhash=ojGk&actionToken=p=p%3Dbiz-company-login%26c%3D23632a14-5702-454f-99f0-001e62aa616c%26m%3Dcompany_feed%26n%3D0&t=a%3DisFolloweeOfPoster%253Dfalse%2526distanceFromActor%253D-1%2526actorType%253D%2526likedByUser%253Dfalse%2526targetId%253D%2526recentCommentUrns%253D%2526targetType%253D%2526sponsoredFlag%253DORGANIC%2526verbType%253Dlinkedin%25253Ashare%2526objectType%253Dlinkedin%25253Acontent%2526totalShares%253D0%2526activityId%253Durn%25253Ali%25253Aactivity%25253A6262886658392223744%2526recentLikerUrns%253D%2526actorId%253Durn%25253Ali%25253Acompany%25253A13268905%2526totalComments%253D0%2526relevanceScore%253D0.0%2526recentCommenterUrns%253D%2526isPublic%253Dtrue%2526time%253D-1%2526totalLikes%253D0%2526objectId%253Durn%25253Ali%25253Acontent%25253AJPEG%25252FIMG%25252F6b7dfed041e04549b2c5fd6b2327878e%2526distanceFromNestedActor%253D-1%26s%3DORGANIC%26u%3Durn%253Ali%253Aactivity%253A6262886658392223744&atv=2&actionType=CLICK

```
which clearly contains the flag

```
the-flag-you-seek-is-NSC{HttP_will_mAkE_yoU_loST}
```

Hence, the flah is **NSC{HttP_will_mAkE_yoU_loST}**.