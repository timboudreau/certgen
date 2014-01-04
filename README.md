Certgen
==============

A script to generate a self-signed certificate with a random passphrase, for
getting a test server up quickly.

For baffling reasons, the security world seems to feel it's an asset that 
creating a self-signed certificate is a cryptic, multi-step process involving
a bunch of incantations and intermediate files - when most of the time you're 
just creating a self-signed cert for a web server, and if you want an actual
trusted certificate, you're buying that from a third-party.

This script simply generates self-signed key and certificate file in one step,
passing the domain on the command-line.

Requires [NodeJS](http://nodejs.org), OpenSSL, and a pre-existing 
temporary folder at ``/tmp``.
