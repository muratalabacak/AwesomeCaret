AwesomeCaret
============
AwesomeCaret is a plugin for jQuery.

The usage
=========

the HTML

<code>&lt;input type="text" id="myinput" value="0123456789" /></code>
<code>&lt;br /></code>
<code>&lt;input type="text" id="myinput2" value="0123456789" /> &lt;span id="caretpos">0-0&lt;/span></code>

<code>$(document).ready(function() {
	// will be selected: "23"
	$("#myinput").caret(2, 4);
	
	$("#myinput2").bind("keyup", function() {
		$("#caretpos").html( $(this).caret().start+"-"+$(this).caret().end );
	});
});
</code>
