CSV-REST
========

A RESTful interface to CSV files in PHP. Compatible with CouchDB

Credits
-------

This is a modification of [CSV to API](https://github.com/project-open-data/csv-to-api)  that works with
[CouchGrid](https://github.com/ctzurcanu/CouchGrid)

Requirements
------------

* PHP
* APC (optional)

Usage
-----

1. Copy `class.csv-to-api.php` and `index.php` to your web server.
2. Load a CSV file via the URL `index.php`, using the arguments below.

Arguments
---------

* `source`: the URL to the source CSV
* `source_format`: if the url does not end in `.csv`, you should specify 'csv' here (to facilitate future functionality)
* `format`: the requested return format, either `json`, `xml`, or `html` (default `json`)
* `callback`: if JSON, an optional JSONP callback
* `sort`: field to sort by (optional)
* `sort_dir`: direction to sort, either `asc` or `desc` (default `asc`)
* any field(s): may pass any fields as a key/value pair to filter by

Demo
----

License
-------
GPLv3 or later.
