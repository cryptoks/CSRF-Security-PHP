# CSRF-Security-PHP

This simple code of PHP help to prevent CSRF attacks and injections
<br>

# What is CSRF Attack ?
Cross-Site Request Forgery (CSRF) is an attack that forces an end user to execute unwanted actions on a web application in which they're currently authenticated.
<br>
# Usage
This class has just 3 functions called setToken(), checkToken(), flushKeys().
<br>
# setToken()
setToken() function is used to generate random token. 
# Example
``` php
<?php 
  include("csrf.php");
?>
<form action="" method="post">
    <input type="hidden" name="_token" value="<?php echo csrf::setToken();?>"/>
</form>
```
