# About #

Purr is a jQuery plugin for dynamically displaying unobtrusive messages in the browser. It isdesigned to behave much as the Mac OS X program "Growl." Other simliar plugins exist: [jQuery Growl](http://www.fragmentedcode.com/jquery-growl/), [jGrowl](http://www.stanlemon.net/projects/jgrowl.html), but Purr functions quite differently than both of these by accepting an object to turn into a notification instead of building the notification from a series of parameters. This frees the developer to define whatever setup process he wants and keeps all styling external.

Purr is also different in its presentation of the notices. These can be set to fade out on a timer or stay in place until the user decides to close them. In addition, non-sticky notices won't begin their fade out timers until they are the top non-sticky notice in the list. This gives users a better opportunity to read messages that were added close together.

# Compatability #

Purr has been successfully, though not extensively, tested on IE7, FF2, FF3, Safari3 Windows, and Opera 9.

# Requirements #

  * [jQuery](http://www.jquery.com/) (tested with 1.2.6)

# Documentation #

You can view the [Usage](Usage.md) to learn how to setup and run Purr, or you can view the [Parameters](Parameters.md). For examples, please visit [Purr's home on The Kitchen @ Net Perspective](http://kitchen.net-perspective.com/open-source/purr/).