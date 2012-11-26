SASS Toolkit
============

SASS Toolkit makes developing websites with SASS easier. There are 2 parts of the SASS Toolkit:

1.  **Reset.** The reset removes the browser default styles and fixes various quirks to give developers a consistent starting point when building websites.
2.  **Tools.** The tools are provided to get you up and running faster. A bunch of variables and mixins have been created to deal with common CSS code patterns such as clearfix, generated content, and browser prefixes.

Built for mobile & responsive
-----------------------------

SASS Toolkit has been specifically built for for mobile and responsive sites that are aimed at modern browsers. It uses the `border-box` box model, and out of the box you get responsive images which look great on any sized device, support for HTML5, and mixins for common CSS3 patterns.

Using SASS Toolkit
------------------

To recompile the toolkit sass -> css for the test page:

    sass --watch test/sass/:test/css/

Browser Support
---------------

Not sure, I’ve done limited testing. My guess is IE8+ and the rest.