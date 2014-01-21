Kickstart Sculpin (Static HTML Site)
====================================

TL;DR
=====

# Install

    composer install
    php bin/phing compile

Info
====

This site uses PHP Sculpin app to build a static site.

Dynamic files that should be edited are in source directory.

General process when working with Sculpin is to edit the 'source' files, then publish.

Your able to kick up a dev server on the fly

    php bin/sculpin generate --watch --server

Public files (can be the webroot in servers) will be renderd to the public directory.

**IMPORTANT:** The public dir will be wiped when building. Edit the source files only.

Installing
==========

To install, we can use composer. Ensure composer is installed first, then you can use the
install command. That will add the phr bin to the bin folder for you.

    composer install

Building / Updating
===================

After changes to src are made, run the following command to build the public files from source.

Prod (updates the public direcory)

    php bin/phing publish

Development (local server that creates an 'output_dev' directory)

    php bin/sculpin generate --watch --server

References
==========

- https://sculpin.io/getstarted/

