Resources
=========
The following are the ``resources:``

1. :ref:`Root <root_section>`
2. People
3. Films
4. Starships
5. Vehicles
6. Species

.. _root_section:

Root
----

The **Root** resource provides information on all available *resources* within the API.

Example request:
https://swapi.dev/api/

Example response:
 
HTTP/1.0 200 OK
Content-Type: application/json

{   
"films": "https://swapi.dev/api/films/",
"people": "https://swapi.dev/api/people/",
"planets": "https://swapi.dev/api/planets/",
"species": "https://swapi.dev/api/species/",
"starships": "https://swapi.dev/api/starships/",
"vehicles": "https://swapi.dev/api/vehicles/"
} 

Attributes
++++++++++

* films string -- The URL root for Film resources
* people string -- The URL root for People resources
* planets string -- The URL root for Planet resources
* species string -- The URL root for Species resources
* starships string -- The URL root for Starships resources
* vehicles string -- The URL root for Vehicles resources