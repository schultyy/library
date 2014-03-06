# curl-shortcuts
## Querying CouchDB

    curl -XGET "http://localhost:5984/db/_design/design-doc/_view/my_fancy_view"

### Querying with start and endkey

    curl -XGET "http://localhost:5984/db/_design/design-doc/_view/my_fancy_view?startkey\=\[\"val\"\]?endkey=\[\"val\",\{\}\]"
    
## Query with accept header

    curl -XGET -H "Accept: application/xml" "http://localhost:3000/foo/bar/gedoens"

## Query with Content-Type header

    curl -XGET -H "Content-Type: application/xml" "http://localhost:3000/foo/bar/gedoens"
