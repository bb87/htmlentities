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

# Examples

	var string = "I–t‘rn‰ti™nˆliz¾ti¿n";
	var res = htmlentities.encode(string);
	console.log(res);
	// -> I&ntilde;t&euml;rn&acirc;ti&ocirc;n&agrave;liz&aelig;ti&oslash;n

	var string = "I&ntilde;t&euml;rn&acirc;ti&ocirc;n&agrave;liz&aelig;ti&oslash;n";
	var res = htmlentities.encode(string);
	console.log(res);
	// -> I–t‘rn‰ti™nˆliz¾ti¿n

# Encodings

The following encodings are supported:

* __UTF-8__ (aliased __utf8__)

