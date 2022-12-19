.. StarWars documentation master file, created by
   sphinx-quickstart on Thu Dec 15 15:02:32 2022.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to the SWAPI Documentation!
===================================

This documentation should help you familiarise yourself with the resources available and how to consume them with HTTP requests. If you're after a native helper library then I suggest you scroll down and check out what's available. Read through the getting started section before you dive in. Most of your problems should be solved just by reading through it.

Getting started
---------------

Let's make our first API request to the Star Wars API!
Open up a terminal and use curl or httpie to make an API request for a resource. In the example below, we're trying to get the first planet, Tatooine:
http swapi.dev/api/planets/1/

Base URL
++++++++

The Base URL is the root URL for all of the API, if you ever make a request to swapi and you get back a 404 NOT FOUND response then check the Base URL first.

Rate limiting
''''''''''''''

Swapi has rate limiting to prevent malicious abuse (as if anyone would abuse Star Wars data!) and to make sure our service can handle a potentially large amount of traffic. Rate limiting is done via IP address and is currently limited to 10,000 API request per day. This is enough to request all the data on the website at least ten times over. There should be no reason for hitting the rate limit.

Authentication
!!!!!!!!!!!!!!!

Swapi is a completely open API. No authentication is required to query and get data. This also means that we've limited what you can do to just GET-ing the data. If you find a mistake in the data, then tweet the author or email him.

The Base URL for swapi is:
https://swapi.dev/api/


.. toctree::
   :maxdepth: 2
   :caption: Overview
   
   overview
   beforeyoubegin

.. toctree::
   :maxdepth: 2
   :caption: Policies and Terms

   policiesandterms

.. toctree::
   :maxdepth: 2
   :caption: Developer Guide

   developersguide
   
.. toctree::
   :maxdepth: 2
   :caption: Core resources

   coreresources

.. toctree::
   :maxdepth: 2
   :caption: Webhook Endpoints

   webhookendpoints

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`


