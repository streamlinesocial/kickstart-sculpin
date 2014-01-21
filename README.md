Kickstart Phrozn (Static HTML Site)
===================================

TL;DR
=====

# Install

    composer install
    php bin/phing compile

Info
====

This site uses PHP Phrozn app to build a static site.

Dynamic files that should be edited are in src directory.

General process when working with Phing is to edit the 'src' files, then compile.

Combiling will parse the files in the 'src' dir, and render HTML with them.

Public files (can be the webroot in servers) will be renderd to the public directory.

**IMPORTANT:** The public dir will be wiped when building. Edit the src files only.

Installing
==========

To install, we can use composer. Ensure composer is installed first, then you can use the
install command. That will add the phr bin to the bin folder for you.

    composer install

Building / Updating
===================

After changes to src are made, run the following command to build the public files from src

    php bin/phing compile

Local Server
============

You can use PHP's built in server for development. For example, create a server that listens
to port 12888 (so you can use local http://localhost:12888) use...

    php -S 0.0.0.0:12888 -t public

References
==========


