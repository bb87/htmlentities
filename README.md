htmlentities.js lets you deal with "complex" HTML entities (not just the usual '<' '>' '"' and '&' special characters).

[Demo](http://alexduloz.github.io/htmlentities/demo.html)

# Install

## On the server

`$ npm install htmlentities`

`var htmlentities = require('htmlentities');`

## In the browser

`<script src="htmlentities.js"></script>`

# Methods

## `.encode(string[, encoding])`

Returns the encoded version of `string`. If omitted, `encoding` defaults to `UTF-8`.


## `.decode(string[, encoding])`

Returns the decoded version of `string`. If omitted, `encoding` defaults to `UTF-8`.

# Encodings

The following encodings are supported:

* __UTF-8__ (aliased __utf8__)

