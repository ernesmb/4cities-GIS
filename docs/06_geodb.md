# Geospatial Databases: PostGIS

A geospatial database is basically a very handy tool for storing data that has a spatial component. As other ([relational](https://en.wikipedia.org/wiki/Relational_database)) databases, it stores data in tabular format, where each **table** is structured in: 

* **Rows** represent each occurence of the data we're storing.
* **Columns** represent the attributes associated to each row. 

What makes a geospatial database _geospatial_ is that in addition to numbers, text, arrays and booleans, it can store and operate with a special data type, that represent the shape and location of objects in the surface of Earth. 

As you may know already, one can _ask questions_  to a database, using a language called `SQL` (Structured Query Language). Using `SQL`, we could filter, aggregate and order our data, but also transform it or obtain calculated columns. 
The kind of _questions_ we can _ask_ a geospatial database are something like: 

- _Which houses are closer than 100m from a Metro station?_
- _How many accidents happened in this segment of the street in the last year?_ 
- _Where are the 10 closest grocery stores from this location?_
- _What's the tree species distribution like in this park?_

Using a database (instead of files) to store data has many advantages, as it allows storing and querying bigger volumes of data in a more organized, structured and performant way.

## PostGIS
[PostGIS](http://postgis.net/) is an Open Source extension that adds geospatial capabilities (data types, functions and operators) to a [PostgreSQL](https://www.postgresql.org/) database. 

PostGIS is the foundation for many other projects, such as CARTO.

Take a look at [this amazing talk](https://www.youtube.com/watch?v=g4DgAVCmiDE) from [Paul Ramsey](http://blog.cleverelephant.ca/about), one of the main contributors to the PostGIS project. It can get a bit too technical, but it's a really great introduction to PostGIS and geospatial databases in general. 


## Resources

Other useful links:

* [PostGIS Project](http://postgis.net/) and [official docs](http://postgis.net/docs/manual-2.5/)
* [WKT encoding](https://en.wikipedia.org/wiki/Well-known_text) 
* [Modern SQL](http://modern-sql.com/slides) 
* [Use the Index, Luke](http://use-the-index-luke.com)
* [Pattern matching expressions](https://www.postgresql.org/docs/9.5/static/functions-matching.html)
* [Fill the gaps between two geometries](http://bl.ocks.org/jsanz/60050dbfe104da69f15e)
* [Jump across the Date Line](https://carto.com/blog/jets-and-datelines)
* EPSG codes databases:
  	* [http://epsg.io/](http://epsg.io/)
  	* [http://spatialreference.org/](http://spatialreference.org/)
* [Free your maps from Web Mercator](https://carto.com/blog/free-your-maps-web-mercator/)
* [Stored procedures that return the Antipode's point for an input geometry](https://github.com/geoinquietosvlc/antipodes-map/blob/master/pgsql/funciones.sql)


## Exercise

* [Introduction to Spatial SQL](spatial_sql.md)