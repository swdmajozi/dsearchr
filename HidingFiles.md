# Hiding Files. #

**Go to line 20 of search.php**

**Line 20:
```
if(($file != ".") and ($file != "..") and ($file != ".DS_Store") and ($file != "search.php"))
```** Add:
```
 and ($file != "FILE TO HIDE")
```
before the last ")".

**Example:
```
if(($file != ".") and ($file != "..") and ($file != ".DS_Store") and ($file != "search.php") and ($file != "FILE TO HIDE"))
```**Notes: