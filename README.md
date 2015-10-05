# foundationdotjs
Foundation.js v3.0, just another JavaScript framework.

Foundation.js is a small JavaScript framework designed to make the lives of the developer, webmaster and client easier. Along the way it achieves the holy grail of class-centric JavaScript: the Super keyword. It also provides the very basic interfaces for creating JavaScript objects that easily interact with page elements and provide localizable resources and multi-lingual support.

Foundation is foremost designed to be light weight and modular. Combine the pieces that are needed, leave out the pieces that are not. To make that process easier, Foundation.js defines the ClientLoader class, an extendable class that makes dynamicaly including required scripts into a page easy for the webmaster, easy for the object developer, and seemless to the client. The other great classes in Foundation.js are there only because they are used by loaders, but happen to be very handy for all sorts of classes as well.

Foundation.js is not a "do everything" collection, nor is it "JavaScript's greatest hits". It is a bare minimum, designed to be small, static, and easy on the processor. Although very easy to use, it is designed for JavaScripters frustrated with the language's lack of class-centric inheritance.

Foremost, Foundation.js makes extending classes a breeze. This is extending in the traditional sense; the parent class constructor is automaticaly called (as is it's parent class' constructor, and so on up the chain), and methods from the parent class that were overridden can be called uing the Super keyword as programmers expect. Foundation.js also makes inheriting methods (in the traditional JavaScript sense) easy as well.

Also, some much-needed methods are added to the String prototype:
htmlEncode: Get the HTML encoded value of a string.
urlEncode: Get the URL encoded value of a string.
cEncode: Get the C-language encoded value of a string.
trim: Eliminate white space at the beginning and end of a string.
These methods should be native, and why they continue to be missing is a complete mystery. Instead, String continues to have native methods like sup (sigh).

To start, take a look at how a class is built using the framework:
Foundation.createClass

Also, there are a few basic classes defined:
Foundation.StringBuilder: Build strings fast.
Foundation.Elemental: Methods for two-way interaction with HTML elements.
Foundation.Resourceful: Methods for handling resources, such as language packs.
Foundation.ClientLoader: Class to load the latest version of a complex class and its dependencies on demand.

The above functionality is all contained in the Foundation.js script. In addition, there are several other classes that can be included in a page as weill.

Foundation.Server.js provides easy AJAX function calls to the server.
Foundation.Console.js, a class to write debugging messages to a page.
Foundation.MenuControl.js, easy dropdown menu, clamshell and treeview menu classes.
Foundation.TabControl.js, easy tab class.
Foundation.MicroLogin.js, a class to create a small, overlayed login form on a page.
Foundation.Completer.js, a class to give text input elements completion (the user starts typing, the completer pops down a list to choose from).
