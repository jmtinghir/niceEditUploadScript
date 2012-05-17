niceEditUploadScript
====================

An upload script to Imageshack for NiceEdit rich text editor http://www.nicedit.com

This is the script (nicUpload.php) I developed to upload images directly to imageshack without using the default one on files.nicedit.com which is not working anymore. It is based on Brian's local upload script.

Developed by Jean-Marie Tinghir : http://jmtinghir.net
Based on Brian Kirchoff's upload script.


Instructions
------------
It requires the Imageshack API class imageshack.class.php (http://code.google.com/p/imageshackapi/)

In nicUpload.php, you have to set your own Imageshack API key on the line : ```define('API_KEY', 'Your Imageshack API key');```

Then you simply have to change the js that instantiate an editor to set the upload script url :
```javascript
var editor = new nicEditor({
			[...]
			uploadURI: 'your upload script url'
			[...]
		});
```