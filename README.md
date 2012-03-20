CKEditor Languages Plugin
=========================

This plugin makes is possible to surround contents with &lt;span lang&gt; elements. This is an important requirement for accessibility purposes.

Installation
------------

1. Create a folder named "plugins/languages" into your CKEditor installation.
2. In the CKEditor configuration file (config.js) add the following code:

        config.extraPlugins = 'languages';
    
        // The languages you want to support (code:name).
        config.languages = [ 'fr:French', 'es:Spanish', 'it:Italian' ];

3. Add the "Languages" item to your toolbar.

It's also recommended to append some style to &lt;span lang&gt; elements, so users will be able to notice text with language. For that, you may add something like the following to contents.css:

    span[lang]
    {
       font-style: italic;
    }

License
-------

Licensed under the terms of any of the following licenses at your choice: [GPL](http://www.gnu.org/licenses/gpl.html), [LGPL](http://www.gnu.org/licenses/lgpl.html) and [MPL](http://www.mozilla.org/MPL/MPL-1.1.html).

See LICENSE.md for more information.
