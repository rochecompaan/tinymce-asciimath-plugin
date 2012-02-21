Introduction
============

A TinyMCE plugin to enter ASCIIMath in the TinyMCE Wysiwyg Editor.

It is based on the TinyMCE plugin written by David Lippman as part of
the IMathAS project: http://www.imathas.com/. A demo of the IMathAS
version of the plugin is available here:
http://www.imathas.com/editordemo/demo.html

This version of the plugin has been modified to always render MathML and
not use any fallbacks that generate images server-side. Instead it
assumes you are using MathJax for cross-browser rendering of MathML.

Additionally it uses the latest version (ver 2.0) of the ASCIIMATH
javascript library by Peter Jipsen available here:
http://mathcs.chapman.edu/~jipsen/mathml/asciimath.html

This plugin was developed as part of the FullMarks project funded by the
Shuttleworth Foundation, an open educational repository of model
questions and answers. See http://www.fullmarks.org.za and
http://github.com/fullmarks for more information.

Installation
============

1. Clone the repo to a location relative to your project

2. Install MathJax. See http://www.mathjax.org/docs/1.1/installation.html

3. Copy the plugin to jscripts/tiny_mce/plugins/asciimath directory into your
   TinyMCE plugins directory.

4. Add the plugin to your TinyMCE config, eg:

    <script type="text/javascript">
        tinyMCE.init({
                mode: "textareas",
                plugins: "asciimath",
                theme: "advanced",
				theme_advanced_buttons3: "hr,removeformat,visualaid,|,sub,sup,|,charmap,asciimath",
    });
    </script>

