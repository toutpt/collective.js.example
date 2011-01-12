Introduction
============

This add-on has been done to document the best way to include
a new javascript library into Plone

Plone default javascript libraries
==================================

Plone 4.0: jquery 1.4.X and jquerytools 1.2.5
Plone 3.3: jquery 1.3.2
Plone 3.2: jquery 1.2.6
Plone 3.1: jquery 1.2.6
Plone 3.0: 

Why not jqueryui:
Some core developers think jqueryui is too heavy to be included in Plone
in part because of the css.

Javascript Registry
===================

By default Plone provide a great tool to register and manage
javascripts. I will try here to explain why you must not hard
coded inclusion of javascript libraries.

So what the javascript registry is doing for you:

* Merge javascripts in order and evaluated conditions based on the current page.
* Compress on selected algorithm

For libraries, base your configuration on basic roles: anonymous and authenticated
The result is simple: even if first load need to fetch all libraries used by 
the website, after that nothing else has to be fected because of the cache.

So what happen if I don't do that

#TODO

How to package external a javascript library for Plone
======================================================

#TODO

Optimizations
=============

If you have doubts about javascript registry it is because
you want to optimize javascript resources in your page.


