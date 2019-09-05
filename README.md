# API-understanding
"An application program interface (API) is a set of routines, protocols, and tools for building software applications. Basically, an API specifies how software components should interact" - Webopedia

# White House Web API Standards

* [Guidelines](#guidelines)
* [RESTful URLs](#restful-urls)

## Guidelines

In this document, I will share all links and information that helped me wrap my head around Web APIs. APIs encourage consistency, maintainability, and best practices across applications.

This document borrows heavily from:
* [Roy Thomas Fielding's Dissertation on REST (Chapter 5)](http://www.ics.uci.edu/~fielding/pubs/dissertation/top.htm)
* [Designing HTTP Interfaces and RESTful Web Services](https://www.youtube.com/watch?v=zEyg0TnieLg)
* [API Facade Pattern](http://apigee.com/about/resources/ebooks/api-fa%C3%A7ade-pattern), by Brian Mulloy, Apigee
* [Web API Design](http://pages.apigee.com/web-api-design-ebook.html), by Brian Mulloy, Apigee

## RESTful URLs

### General guidelines for RESTful URLs
* A URL identifies a resource.
* URLs should include nouns, not verbs.
* Use plural nouns only for consistency (no singular nouns).
* Use HTTP verbs (GET, POST, PUT, DELETE) to operate on the collections and elements.
* You shouldn’t need to go deeper than resource/identifier/resource.
* Put the version number at the base of your URL, for example http://example.com/v1/path/to/resource.
* URL v. header:
    * If it changes the logic you write to handle the response, put it in the URL.
    * If it doesn’t change the logic for each response, like OAuth info, put it in the header.
* Specify optional fields in a comma separated list.
* Formats should be in the form of api/v2/resource/{id}.json
