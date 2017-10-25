# 24 OCT 17
### HTTP
HTTP = Hypertext Transfer Protocol

#### HTTP Request
```
GET /index.html HTTP/1.1<CRLF>
Host: www.example.com<CRLF>
<CRLF>
```

#### HTTP Response
```
HTTP/1.1 200 OK<CRLF>
Date: Mon, 23 May 2005 22:38:34 GMT<CRLF>
Server: Apache/1.3.3.7 (Unix) (Red-Hat/Linux)<CRLF>
Last-Modified: Wed, 08 Jan 2003 23:11:55 GMT<CRLF>
Etag: "3f80f-1b6-3e1cb03b"<CRLF>
Accept-Ranges:  none<CRLF>
Content-Length: 438<CRLF>
Connection: close<CRLF>
Content-Type: text/html; charset=UTF-8<CRLF>
<CRLF>
<438 bytes of content>
```

#### HTTP Methods
GET
POST
PUT
DELETE

Safe <-> Unssafe
GET  --- POST PUT DELETE
