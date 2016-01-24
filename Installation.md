# Installation: #
## With form validation ##
  1. **Copy & Paste:**
```
<script type="text/javascript">
function validate_required(field,alerttxt)
{
with (field)
  {
  if (value==null||value=="")
    {
    alert(alerttxt);return false;
    }
  else
    {
    return true;
    }
  }
}

function validate_form(thisform)
{
with (thisform)
  {
  if (validate_required(search,"Please enter somthing to search.")==false)
  {search.focus();return false;}
  }
}
</script>
```
immediately before the `</head>` tag.
  1. **Copy & Paste:**
```
<form id="FormName" action="search.php" method="post" name="FormName" onsubmit="return validate_form(this)">
			<strong><span class="ds7">Search:</span></strong>  <input class="dsR2" type="search" name="search" results="5" size="25" accesskey="S"><br></form>
```
in between the `<body>` and `</body>` tags.

## Without form validation ##
  1. **Copy & Paste:**
```
<form id="FormName" action="search.php" method="post" name="FormName" >
			<strong><span class="ds7">Search:</span></strong>  <input class="dsR2" type="search" name="search" results="5" size="25" accesskey="S"><br></form>
```
in between the `<body>` and `</body>` tags.