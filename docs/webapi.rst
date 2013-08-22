Web API
========

The following document explains the current Web API, remember this project
is under heavy development, so the API inputs might change a lot.


Creating a new component
-------------------------

- Request type: *POST*
- URL:          */component/*

Post data:
::

	{
	   "description":"description of the component",
	   "name":"Name",
	   "product_id":1,
	   "user":"user@example.com",
	   "password":"asdf",
	   "owner_id":1
	}

Get component list for a product
---------------------------------

- Request type: *POST*
- URL:          */components/*

Post data:
::

	{ 
		"product_id": 1
	}

Output:
::

	{
	   "0ad":[
	      "522",
	      "0ad",
	      "Cross-Platform RTS Game of Ancient Warfare"
	   ],
	   "0ad-data":[
	      "523",
	      "0ad-data",
	      "The Data Files for 0 AD"
	   ],
	   "0xFFFF":[
	      "524",
	      "0xFFFF",
	      "The Open Free Fiasco Firmware Flasher"
	   ],
	   "389-admin":[
	      "525",
	      "389-admin",
	      "Admin Server for 389 Directory Server"
	   ]
	}