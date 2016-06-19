warc: Python library to work with WARC files (Especially for Clueweb Datasets)
============================================

.. image:: https://secure.travis-ci.org/anandology/warc.png?branch=master
   :alt: build status
   :target: http://travis-ci.org/anandology/warc

Introduction
------------

`ClueWeb09 <http://www.lemurproject.org/clueweb09.php/>`_ and `ClueWeb12 <http://www.lemurproject.org/clueweb12.php/>`_ dataset consists of
~1 billion web pages crawled in January and February 2009 and 2012.

It is used by several tracks of the `TREC <http://trec.nist.gov/>`_ conference.

Notification
------------

This library is a fork of
`internetarchive/warc <https://github.com/internetarchive/warc>`_
`cdegroc/warc-clueweb <http://github.com/cdegroc/warc-clueweb>`_
that can handle both ClueWeb09 and ClueWeb12 dataset.

Why I change the code?

    1. there are certain caveats with ClueWeb09's files.
       it does not use the standard \\r\\n end-of-line markers.
       Moreover, some records are
       `ill-formed <http://lintool.github.com/Cloud9/docs/content/clue.html#malformed>`_.

    2. `cdegroc/warc-clueweb <http://github.com/cdegroc/warc-clueweb>`_ 
       This fork repo could not handle Clueweb12 dataset and another issue is that it could miss
       1-2 document when dealiing every .warc.gz file

Documentation
-------------

Only minor modifications to the original library were made.

The original documentation of the warc library still holds.

The documentation of the warc library is available at http://warc.readthedocs.org/.

How to use
----------

For simply analyze warc format files such as clueweb09 and clueweb12, you can just use warc/warc.py

For other usage, just reference original document.
	
License
-------

This software is licensed under GPL v2. See LICENSE_ file for details.

.. LICENSE: https://github.com/RominYue/warc/blob/master/LICENSE
