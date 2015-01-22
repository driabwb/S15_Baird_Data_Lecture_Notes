# Lecture 2

## Markdown

A form of markup language  
useful for plain text to richtext/HTML

2 types in use by github
*Standard Markdown (SM)
*Github Flavoured Markdown (GFM)

What can you do with it?
* Styling
* Word formatting
* Add images
* Lists (ordered and unordered)
* Links
* Code blocks

### Headers
use pound '#'
consecutive create sub headers through 6

### Codeblocks
surround by three back ticks

provide syntax highlighted by specifing language after first set of backticks

### Tables
Pipes seperate columns  
there exist methods to specifying alignment

# Horizontal Lines
This will happen with 3 of either # * or _ (underscore)

## Services

Web browser
* Send HTTP request
  * Get
  * Post
  * Delete
  * Put

Web/App server
1. gives to a handler
  * generates a response of some form
2. send HTTP response

### RESTful
* Representation(Resource) E
* An Architecture for service base app
* Resources are specified by by URI
  * Resources have CRUD operations
    * Create
    * Read
    * Update
    * Destroy

Image have a site with info about users  
/users/{id}

Can call HTTP ops on any given resource

* Get -> Read
* Post -> Create (a user) { takes data }
* Put -> Update (on a particular user)
* Delete -> Destroy (a particular user)

### Example of a Simple Service

#### Consideration
* Database
* ids
* inputs (what are they what format)
* outputs (What are they what format)
* Errors
