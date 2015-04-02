# Lecture 3: Restful Web Service

Code for this is available in the org. github.

More Assignment info to come.

## REST
* Architectural style
  * formalized by Roy Fielding UC Irvine
* Developing web service
* Alternative SOAP
  * Very complex
  * Attempt to be more formal
* service provide access to linked set of resources
* preform ops similar to HTTP spec
  * CRUD ops (See Lecture2.md) 

### Examples

* GET /api/1.0/users
  * Retrieve list all users
* Get /api/1.0/users/0
  * Retrieve details of user 0
* POST /api/1.0/users
  * Create
  * more details in POST body
* PUT /api/1.0/users/0
  * Update user 0
* Delete /api/1.0/users/0
  * Delte user 0


Good practice to format with prefix /<API>/<version>/

### Discussion
* each op may produce a result
* POST and PUT typically send data
  * Also in JSON format
  * May be in URL or body of HTTP Request
* if auth needed
  * auth data in HTTP headers

## Issues
* Security
* Identity
* Failure
* Persistence
