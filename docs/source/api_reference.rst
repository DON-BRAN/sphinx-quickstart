API
===

.. currentmodule: simpleble


.. autosummary::
   :toctree: _autosummary
   :template: class.rst
   
 
   Getting started with Crawler is easy.
   The main class you need to care about is crawler.main.Crawler

   crawler.main

   automodule: crawler.main
   Crawler Python API

   Getting started with Crawler is easy.
   The main class you need to care about is crawler.main.Crawler

   crawler.main

   crawler.utils

   crawler.utils.should_ignore

   should_ignore(['blog/$'], 'http://ericholscher.com/blog/')
   True

   # This test should fail
   should_ignore(['home'], 'http://ericholscher.com/blog/')
   True

   crawler.utils.log

   log('http://ericholscher.com/blog/', 200)
   OK: 200 http://ericholscher.com/blog/ 

   log('http://ericholscher.com/blog/', 500)
   ERR: 500 http://ericholscher.com/blog/

   # This test should fail
   log('http://ericholscher.com/blog/', 500)
   OK: 500 http://ericholscher.com/blog/
