# Bootstrap Better Typeahead Extension

This **Bootstrap Better Typeahead** extends the Bootstrap Typeahead plugin and adds support for a ```minLength``` option set to zero.

Setting ```minLength``` to zero now correctly opens the full list of available options on element focus and on empty queries.

#### Adding the extension to your Bootstrap application

Adding the plugin is unobtrusively - ie. you extend the bootstrap plugin by adding the following file after you included the original bootstrap plugin.

#### Example

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Bootstrap Better Typeahead Example</title>

        <!-- optional -->
        <link rel="stylesheet" href="/css/bootstrap-better-typeahead.css">
    </head>
    <body>
        <input type="text" id="selector">

        <script type="text/javascript" src="//ajax.googleapis.com/ajax/libs/jquery/2.0.0/jquery.min.js">
        <script type="text/javascript" src="//raw.github.com/twitter/bootstrap/master/js/bootstrap-typeahead.js">

        <script type="text/javascript" src="/js/bootstrap-better-typeahead.js">
        
        <script type="text/javascript">
            $(function() {
                $("#selector").typeahead({
                    minLength: 0,
                    source: ["Neque", "porro", "quisquam", "est", "qui", "dolorem", "ipsum", "quia", "dolor", "sit", "amet", "consectetur"]
                });
            });
        </script>
    </body>
</html>
```

#### Licence

Copyright (C) 2013 Philipp Nolte

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.