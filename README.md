Sass Toolkit
============

Sass Toolkit makes developing websites with Sass easier. There are 2 parts of the Sass Toolkit:

1.  **Reset.** The reset removes the browser default styles and fixes various quirks to give developers a consistent starting point when building websites.
2.  **Tools.** The tools are provided to get you up and running faster. A bunch of variables and mixins have been created to deal with common CSS code patterns such as clearfix, generated content, and browser prefixes.

Built for mobile & responsive
-----------------------------

Sass Toolkit has been specifically built for for mobile and responsive sites that are aimed at modern browsers. It uses the `border-box` box model, and out of the box you get responsive images which look great on any sized device, support for HTML5, and mixins for common CSS3 patterns.

Installing Sass Toolkit In An Existing Project
----------------------------------------------

    git remote add sass-toolkit git://...
    
    git fetch
    
    git merge sass-toolkit/master
    
    # Move the sass directory whereever you like.
    mv sass/ assets/

Updating Sass Toolkit
---------------------

    git fetch sass-toolkit
    
    git merge sass-toolkit/master

Using Sass Toolkit
------------------

To recompile the toolkit Sass -> css for the test page:

    sass --watch test/sass/:test/css/

Browser Support
---------------

Not sure, I’ve done limited testing. My guess is IE8+ and the rest.