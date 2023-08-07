# Authentication

Metronero API uses bearer tokens passed via `Authorization` header. A merchant must register and/or login to issue a token.

## POST /register
### Response

## POST /login
### Response

## POST /logout
Invalidates the current bearer token. If the supplied token is already invalid/expired, does nothing.
### Response
