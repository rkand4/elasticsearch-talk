# More like this

## Register a "more like this" query

More like this (or MLT) queries allow you to find documents that are "like" a document you specify, containing a similar string or description.

This request will return all documents with similar names,"about" fields, or descriptions as the lake_shore_drive wikipedia page.

`GET /wikipedia/locations/lake_shore_drive/_mlt?name,about,description&min_doc_freq=1 `

## Limit the terms shown in the results

You may not necessarily want to see ALL of the information returned by the "more like this" query.

`GET /wikipedia/locations/lake_shore_drive/_mlt?name,about,description&min_doc_freq=1 `

```json
{
    "fields" : ["about"]
}
```