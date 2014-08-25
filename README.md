data_structure_html
===================

php class to truncate HTML content , 

INSTALLATION 

just upload the helpers folders to the blesta directory . 

USAGE

inside the controller add :

$this->set("html", $this->DataStructure->create("html"));

in the template file .PDT you can use it as the fallowing code 

$result = $html->truncate($text,  $length = 150 , $strip_tags = true , $ending = ' ... ', $exact = false, $considerHtml = true  );

you can sipmly you it as 

$result = $html->truncate($this->Html->ifSet($vars->text),  180   );

the class support the fallowing param 

	 @param string $text HTML to truncate.
	 @param integer $length Length of returned string, including ellipsis.
	 @param boolean $strip_tags If true , $text will rendered without html tags 
	 @param string $ending Ending to be appended to the trimmed string.
	 @param boolean $exact If false, $text will not be cut mid-word
	 @param boolean $considerHtml If true, HTML tags would be handled correctly
	 
	 
this class is taken from the CakePHP framework .




