# HTMLEncode

A Xojo module for encoding/decoding HTML entities

Inspired by the HTMLEntities module originally created by [Thom McGrath][original].
Rewritten to use faster Dictionaries and I have migrated as much of the code as
is currently possible to the new Xojo framework.

## About ##

Certain characters need to be encoded if they are to be displayed in a HTML
document. These are known as HTML entities. This module will convert these
characters into their respective HTML symbols and back again.

## Usage ##

```xojo
using HTMLEncode

dim raw as Text = "<p>Copyright © 2016</p>"
dim encoded as Text = raw.EncodeEntities()

' result is:
' &lt;p&gt;Copyright &copy; 2016&lt;/p&gt;
```

[original]: https://www.thezaz.com/blog/real_studio/converting_html_entities/
