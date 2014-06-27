jquery.simpleTabs
=================

Minimalist, markup agnostic and design free plugin for tabs functionality.
It has no config options, or fancy effects. Will update tabs on hash change, when supported, with no polyfill.
Active anchor tag will receive a class of 'is-active'. Default tab, when initializing plugin, will respect following priority:

1. Current hash;
2. Anchor that has 'is-active' class;
3. First anchor in the list.

That is about all you will get for 1KB.

Usage
-----

Load jQuery;
Load the plugin;
Call the simpleTabs method from the element containing links to existing IDs:

    <script src="http://code.jquery.com/jquery-1.11.1.min.js"></script>
    <script src="jquery.simpleTabs.min.js"></script>

    <ul id="list-of-links">
        <li><a href="#tab01">Tab 01</a></li>
        <li><a href="#tab02">Tab 02</a></li>
        <li><a href="#tab03">Tab 03</a></li>
        <li><a href="#tab04">Tab 04</a></li>
    </ul>
    
    <div id="tab01">
        <h2>This is tab 01</h2>
    </div>
    <div id="tab02">
        <h2>This is tab 02</h2>
    </div>
    <div id="tab03">
        <h2>This is tab 03</h2>
    </div>
    <div id="tab04">
        <h2>This is tab 04</h2>
    </div>
    
    <script type="text/javascript">
        $("#list-of-links").simpleTabs();
    </script>
