# Read: 12 - Spring RESTful Routing & Static Files

## Baeldung: Spring Request Mapping

![Request Mapping by Path](img/requestMapping2.PNG)

![Request Mapping the HTTP Method](img/requestMapping3.PNG)

![Request Mapping with headers Attribute](img/requestMapping4.PNG)

![Request Mapping Consumes and Produces](img/requestMapping5.PNG)

![Single @PathVariable](img/requestMapping6.PNG)

![Multi @PathVariable](img/requestMapping7.PNG)

![Request Mapping Request Parameters](img/requestMapping8.PNG)

![Request Mapping by multiple path mapped to the same controller method](img/requestMapping9.PNG)

![Request Mapping Multiple HTTP Request Methods to the Same Controller Method](img/requestMapping10.PNG)

![Request Mapping Fallback for all Request](img/requestMapping11.PNG)

![New Request Mapping Shortcuts](img/requestMapping12.PNG)

![Spring Configuration](img/requestMapping13.PNG)

## Spring guide: Accessing Data with JPA

Just read about the steps and will use it as a template when adding data.

## Baeldung: Comparing repositories

- Different kinds of Spring Data repository interfaces
  - CrudRepository
  - PagingAndSortingRepository
  - JpaRepository
- Each of these defines its own functionality:
  - CrudRepository provides CRUD functions
  - PagingAndSortingRepository provides methods to do pagination and sort records
  - JpaRepository provides JPA related methods such as flushing the persistence context and delete records in a batch
- CrudRepository
![CrudRepository](img/repositories.PNG)
  - Simple and generic, but provides all basic query abstractions needed in an application
- PagingAndSortingRepository
![PagingAndSortingRepository](img/repositories2.PNG)
  - Key for implementing pagination
  - Create Pageable object with certain properties:
    - Page size
    - Current page number
    - Sorting
![PASR2](img/repositories3.PNG)
- JpaRepository
![JpaRepository](img/repositories4.PNG)
  - Interface extends PagingAndSortingRepository which means it has all methods present in the CrudRepository as well.
- Downsides of using repositories
  - Be careful not to expose these internal implementation details
  - Extending CrudRepository exposes a complete set of persistence methods at one. In some circumstances this is not bad.

[Back to README](README.md)
