awkward
=======

Schema files for awkward data
------------------------------------

These schema files create awkward data for testing the UI/UX of
[https://github.com/cloudant-labs/couchdb/tree/fauxton/src/fauxton](fauxton).

Create data using [https://github.com/cloudant-labs/etc/blob/master/gen_docs.py](gen_docs) as follows:

    python gen_docs.py -u $URL -s nested.json

where `$URL` is the full URL of the database to write to.

 * `bigdocs.json`: documents with large chunks of text
 * `longkeys.json`: documents with awkwardly long keys
 * `lotsofviews.json`: documents with lots of views
 * `manyddocs.json`: documents with lots of design docs
 * `nested.json`: documents with a very nested data structure

If you have an idea for an awkward dataset please submit a pull request!
