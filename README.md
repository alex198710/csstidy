CSSTidy
=======
* Wrapper around CSSTidy
* CSSTidy 1.3 csstidy.sourceforge.net


With PHP > 5.3
-----

Composer.json
```
Add this line:
"alex198710/csstidy": "dev-master"
```
Then use it like this:
```
<?php
include('class.csstidy.php');

$css_code = '
a {
color:black;
background-color:blue;
}';

$css = new csstidy();

$css->set_cfg('remove_last_;',TRUE);

$css->parse($css_code);

echo $css->print->formatted();
?>
```
            
            
            
