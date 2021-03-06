Pylons
++++++

What is this fork?
==================

It has been found that some of my personal projects would be more easily
transitioned to Python 3 than to pyramid. Because of this, it may be easier
to also update Pylons and relevant dependencies, and this way wrap my Pylons
applications under Pyramid 1.9+, transitionally adding any new views and lib
utilities via pyramid, updating current libraries to be separate from the
Pylons StackedObjectProxies or additionally with the pyramid regiatry.

The soon deprecation of Python2 is a worse bottleneck than the exisring death
of Pylons.

.. image:: https://secure.travis-ci.org/Pylons/pylons.png?branch=master
   :alt: Build Status
   :target: https://secure.travis-ci.org/Pylons/pylons

Pylons is a rapid web application development framework.

.. note::

    Pylons has merged with repoze.bfg, and is now in maintenance-only
    mode. It's highly recommended that new projects start with the new
    merged web framework, `pyramid <http://www.pylonsproject.org/>`_.

Install
=======

`Read the online Installation instructions
<http://docs.pylonsproject.org/projects/pylons-webframework/en/latest/gettingstarted.html#installing>`_.

If you want to install from source you can run the following command:

.. code-block :: bash

    $ python setup.py install

This will display a message and download setuptools if the module is not
already installed. It will then install Pylons and all its dependencies. You
may need root privileges to install setuptools.

Testing
=======

To test the source distribution run the following command:

.. code-block :: bash

    $ python setup.py test

This will install additional dependencies needed for the tests. As above, you
may need root privileges.

Documentation
=============

`Read the complete Pylons web framework documentation
<http://docs.pylonsproject.org/projects/pylons-webframework/>`_.

`Definitive Guide to Pylons <https://thejimmyg.github.io/pylonsbook/>`_ is a book about Pylons published by Apress, written by James Gardner, with free HTML rendering.

Generating documentation requires Sphinx:

.. code-block :: bash

    $ easy_install Sphinx

Then to build the documentation use the commands:

.. code-block :: bash

    $ cd pylons/docs/<lang>
    $ make html
