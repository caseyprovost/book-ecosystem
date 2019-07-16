## Book Ecosystem
  
The book ecosystem is a project of love and learning by Casey Provost. It is comprised of a suite of JSON:API Spec services, a single GraphQL proxy, and finally a React/Apollo client application that consumes it all. In all of the projects you will find a Dockerfile and a docker-compose file for maximum portability. 

## Master Auth                                                  

*Master Auth* serves as the user authorization system. Think of it like an internal 0Auth. This has all of our user details and credentials.

#### Tech Stack:

* Rails API
* Devise JWT
* Postgres
* Docker

## Bookshelf

*Bookshelf* serves as the a catalog of books. It is used to populate the bookstore. In addition to "cataloging" it also provides book category hierarchy and searching.

#### Tech Stack:

* Rails API
* Graphiti
* Postgres
* Docker

## Bookstore

*Bookstore* serves as the e-Commerce side of this project. It allow users to browse and purchase books ability in the *Bookshelf*.

#### Tech Stack:

* Rails API
* Graphiti
* Postgres
* Docker

## Author Repository

The *Author Repository* serves as a kind of "rolla-dex" of author information including name, biography, basic stats, and photos.

#### Tech Stack:

* Rails API
* Graphiti
* Postgres
* Docker

## Publisher Repository

The *Publisher Repository* serves as a kind of "rolla-dex" of publisher information including name, description, etc.

#### Tech Stack:

* Rails API
* Graphiti
* Postgres
* Docker

## Spider

*Spider* is the glue that holds the system together. **All** API requests from the client **and** microservices go through this. This gives our API clients maximum power by being able to request multiple resources at once through a single request.

#### Tech Stack:

* Rails API
* GraphQL
* Docker
