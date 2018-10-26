.. _bootstrap-label:

=============================
Bootstrapping A Volto Project
=============================

Installing Plone
================

On order to run Volto you need a backend.
This can be either Plone or Guillotina.
For this course we will use Plone, you can download Plone at https://plone.org/download.

Installing Dependencies
=======================

First step is to install the correct Node version using ``nvm``:

.. code-block:: console

    $ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash

Then you can install the latest LTS version of node:

.. code-block:: console

    $ nvm install v8.11.3

We use the package manager ``yarn``, to install do:

.. code-block:: console

    $ npm install -g yarn

And add the ``create-volto-app`` package:

.. code-block:: console

    $ yarn global add @plone/create-volto-app

Bootstrapping A Project
=======================

To create a new volto project type the following:

.. code-block:: console

    $ create-volto-app my-volto-app

It will create a folder called `my-volto-app` inside the current folder with the following structure:

.. code-block:: console

    my-volto-app
    ├── README.md
    ├── node_modules
    ├── package.json
    ├── .babelrc
    ├── .eslintrc
    ├── .gitignore
    ├── .yarnrc
    ├── locales
    ├── public
    │   ├── favicon.ico
    │   └── robots.txt
    ├── theme
    │   └── theme.config
    └── src
        ├── actions
        ├── components
        ├── constants
        ├── customizations
        ├── helpers
        ├── reducers
        ├── client.js
        ├── config.js
        ├── index.js
        └── routes.js

Running The Project
===================

To run the project you can type:

.. code-block:: console

    $ yarn start

This will start the server on port 3000.