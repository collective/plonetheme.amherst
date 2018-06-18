==================
plonetheme.amherst
==================


Introduction
============

*plonetheme.amherst* Theme is an installable Plone_ Theme using the **theming** and **packaging** 
features available in `plone.app.theming`_.


Requirements
============

- From the Plone 4.1.x To the Plone 4.3 latest versión (https://plone.org/download)
- The ``plone.app.theming`` package (*will be installed as a dependency of this package*)


Features
========

- It's an installable Plone_ Theme package.
- After installation from Add-ons controlpanel, this theme is enabled automatically.
- Also it's a simple Diazo_ package (Zip file).
- It's have support for clean uninstallation.


Installation
============


Add Plone site
--------------

Install Plone 4.x with `plone.app.theming`_ and create a Plone site (if you have not already)
with Diazo theming configured.

.. image:: https://github.com/collective/plonetheme.amherst/raw/master/screenshot0.png
  :width: 1024px
  :alt: Create a Plone site from ZMI
  :align: center


Zip file
--------

If you are an end user, you might enjoy installation via zip file import.

1. Download the zip file: https://raw.github.com/collective/plonetheme.amherst/master/amherst.zip
2. Import the theme from the Diazo theme control panel.

.. image:: https://github.com/collective/plonetheme.amherst/raw/master/screenshot1.png
  :width: 1024px
  :alt: Import the Diazo theme zip file
  :align: center


Buildout
--------

If you are a developer, you might enjoy installing it via buildout.

For install ``plonetheme.amherst`` package add it to your ``buildout`` section's 
*eggs* parameter e.g.: ::

   [buildout]
    ...
    eggs =
        ...
        plonetheme.amherst


and then running ``bin/buildout``.

Or, you can add it as a dependency on your own product ``setup.py`` file: ::

    install_requires=[
        ...
        'plonetheme.amherst',
    ],


Select theme
^^^^^^^^^^^^

Select and enable the theme from the Diazo control panel.

.. image:: https://github.com/collective/plonetheme.amherst/raw/master/screenshot2.png
  :width: 1024px
  :alt: For select the Diazo theme just click on Activate button
  :align: center

That's it!

You should see: 

.. image:: https://raw.github.com/collective/plonetheme.amherst/master/plonetheme/amherst/theme/amherst/preview.png
  :width: 1024px
  :alt: plonetheme.amherst preview
  :align: center


Contribute
==========

- Issue Tracker: https://github.com/collective/plonetheme.amherst/issues
- Source Code: https://github.com/collective/plonetheme.amherst


Help
----

Obviously there is more work to be done. If you want to help, pull requests accepted! Some ideas:

* Add a diazo rule to import Plone editing styles
* Configure styles to use portal_css
* Improve styles 


License
=======

The project is licensed under the GPLv2.


Credits
-------

- Andrew Pasquale, (apasquale at healthlens dot org).
- Leonardo J. Caballero G. (leonardocaballero at gmail dot com).

.. _`Plone`: http://plone.org
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
.. _`Diazo`: http://diazo.org
