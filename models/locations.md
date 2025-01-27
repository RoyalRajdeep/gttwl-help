#### LOCATIONS
---

This collection gives you a list of locations that you can use to make a location directory.

Tags available on this page
---------------------------
```
* locations - the list of locations themselves.
* country_codes - a list of countries for a selected content (only available if a continent is selected)
* pagination
```

Location tag detail
-------------------
```
* id
* kind
* title
* short_title - a combined title, you will probably want to use thsi most.
* permalink
* content - use with simple_format filter for better representation
* lat
* lng
* address - full address string
* country_code - eg: "us"
* country_name
* region - eg: "Florida"
* city
* continent - eg: "eu"
* woeid
* place_type
* aliases
* geonameid
* population
* feature_code
* attachments - list of photos or videos
* primary_media - the primary attachment
```

Filtering
---------
You can filter the collection by passing in the following parameters to the url:
```
* continent_code - eg: "EU", if you select this, then all the countries in that continent are also available.
* country_code - filtered by country. eg: "us"
* search - full text for searching places.
You can combine the parameters.
```

INDIVIDUAL LOCATION PAGE
------------------------
All the above tags are available. However we have added a few more for convenience

```
* locations - a list of nearby places (limited to 8)
* blogs - a list of blogs that mention nearby places
* products - a list of products that mention nearby places
* related - a list of products and blogs combined from the 2 above
```
