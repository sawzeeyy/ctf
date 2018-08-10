# Canada : Wobe Nation
**Category:** Web Application
**Points:** 150


## Problem

Well, God save the King.

**Hint:** On the fourth day of the competition\na birth party was announced, you need\nan invite because you cannot gate crash!
**Link:** http://94.156.189.140:9292


## Solution

The link given was to a web app.

Simply sending a GET request to the endpoint returned a cookie. Below is an example of the request sent

```
GET / HTTP/1.1
Host: 94.156.189.140:9292

...
```

And the response was 

```
200 Ok
...
Set-Cookie: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpbnZpdGUiOiJkRGs1WVVoTVRVSk1VRUZwWjBvMWFXWm9abnBwYzJJNVoxSnBUWGhoWjJZNWFIZGhhM1ZRTVdkNGNrNURabGRVUTNFMGMwVT0ifQ.FtT0nz5NrQTuc4xPh7UeguTUgZkL2cjKwhIm0zL9YVg
```

This is JWT in action and surely, the string is base64 encoded.

```
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpbnZpdGUiOiJkRGs1WVVoTVRVSk1VRUZwWjBvMWFXWm9abnBwYzJJNVoxSnBUWGhoWjJZNWFIZGhhM1ZRTVdkNGNrNURabGRVUTNFMGMwVT0ifQ.FtT0nz5NrQTuc4xPh7UeguTUgZkL2cjKwhIm0zL9YVg
```

The string above was decoded to 

```
{"alg":"HS256","typ":"JWT"}.{"invite":"dDk5YUhMTUJMUEFpZ0o1aWZoZnppc2I5Z1JpTXhhZ2Y5aHdha3VQMWd4ck5DZldUQ3E0c0U="fQ.Ôô>M­îsOµäÔÙÈÊÂ&Ó2ýYVg
```

From the hint on the challenge, we need an invite, and Yay! This is an invite
We got invite! 


```
dDk5YUhMTUJMUEFpZ0o1aWZoZnppc2I5Z1JpTXhhZ2Y5aHdha3VQMWd4ck5DZldUQ3E0c0U=

```
Base64 decoded the invite string above and got another encoded string.

```
t99aHLMBLPAigJ5ifhfzisb9gRiMxagf9hwakuP1gxrNCfWTCq4sE
```

This took an awful lot of time to figure but we finally base58 decoded to

```
NSC{awon_omo_wobe_welcome_to_the_party}
```

Hence, the flag is **NSC{awon_omo_wobe_welcome_to_the_party}**.