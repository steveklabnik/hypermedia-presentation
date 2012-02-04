<!SLIDE api-overview>

# API Overview

<!SLIDE three-styles>

# Four major architectural styles

<!SLIDE style-rpc>

# RPC

    POST /jsonrpc
    { "method": "echo",
      "params": 
     ["Hello JSON-RPC"],
      "id": 1
    }

    Response:
    { "result": "Hello JSON-RPC",
      "error": null, "id": 1}

<!SLIDE style-rpc-philosophy>

# RPC

## Make a method call over the internet.

<!SLIDE style-soap>

# SOAP
    POST /soap
    <xml>
      ZOMGSOMUCHSTUFF

    Response: 
    <xml>
      ZOMGSOMUCHSTUFF

<!SLIDE style-soap-philosophy>

# SOAP

## Send an object over the wire.

<!SLIDE rest-disclaimer>

# Remember, I'm speaking about 'Rails REST.'

<!SLIDE style-rest>

# REST

    PUT /posts/1
    &title=Hello%20World

    Response:
    200 OK

<!SLIDE style-rest-philosophy>

# REST

## RPC with a uniform interface

<!SLIDE style-hypermedia>

# Hypermedia

    GET /
    Content-Type: application/collection+json

    { "collection" :
      {
      "links" : [
        {"rel" : "feed",
         "href" : "http://example.org/rss"}
      ],
      ...
    }


<!SLIDE style-hypermedia-philosophy>

# Hypermedia

## Hypertext as the engine of application state

<!SLIDE three-styles>

# RECAP: Four major architectural styles

* RPC
* SOAP
* REST
* Hypermedia
