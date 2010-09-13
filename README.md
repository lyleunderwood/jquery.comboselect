JQuery.comboselect
==================
This is a port and a rehabilitation of the [JQuery.comboselect](http://plugins.jquery.com/project/comboselect) plugin.

What's it do?
-------------
The plugin transforms a multi-select from a single element to side by side multi-selects. You can move selections from one select to another instead of highlighting them in single.  Look at the example. This will make a lot more sense, I assure you.

As part of the transformation, your select is hidden, but updated as you double-click or select and press the add/remove buttons.

Usage
-----
Shown with default options as options
    $(#my_multi_select_box).comboselect({
      addremall : true,  // include the add/remove all buttons
		  add_allbtn: ' &gt;&gt; ',   // label for the "add all" button
      rem_allbtn: ' &lt;&lt; ',    // label for the "remove all" button
		  addbtn: ' &gt; ',   // label for the "add" button
      rembtn: ' &lt; ',    // label for the "remove" button
      cs_container: 'div', //  html tag to contain both comboselects
      btn_container: 'div' // html tag to contain the comboselect buttons
    });


To set for legeacy compatibility, define the following after you include the plugin, but before you 'wire' it to anyting:
    jQuery.fn.comboselect.defaults = {
      addremall : false,
		  addbtn: ' &gt; ',
      rembtn: ' &lt; ',
      cs_container: 'fieldset',
      btn_container: 'fieldset'
    };

This method can be used for any defaults you prefer, so you do not have to set options on each use of the comboselect.