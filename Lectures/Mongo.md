# MongoDB

* Latest Stable is 2.6
* NoSQL DB
* Document based DB
  * Doc consist key and value
* Takes care of balancing data and load on cluster

## Consistency and Transactions

* not multi doc atomic transac supported

## Terms

* Document
  basic unit of data
* Colleciton

## Documents
* self defining
* unordered set keys with assoc values
* keys are utf-8 strings
* cannot use \0
* should not use '.' '$'
* case and type sensitive
* can't have duplicates keys

## Collections
* group of documents
* gives some org to docs
* search more intelligent
* naming convention
* cannot be ""
* cannot have \0
* cannot have system at beginning

## Databases
* one or more collections
* each has own permission

### Reserved Database names
*Admin
  * adim users
* Local
  * never duplicated
