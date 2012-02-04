<!SLIDE lightblue-title padding-bottom>

# Implement!

<!SLIDE lightblue-title padding-bottom>

# Sample response

      request("http://w3clove.com/api/", 
        "application/vnd.w3clove.validation+json")
      # =>  
      {
        "links":[
        {"rel":"website-form", "href":"..."},
        {"rel":"sitemap-form", "href":"..."}
        ]
      }
    

<!SLIDE>

    uri = response["links"].find {|link| 
      link["rel"] == "sitemap-form"
    }["href"]
    
    request(uri,
      "application/vnd.w3clove.validation+json")
    # => 
    {
      "forms":[
        {"href":"...", 
         "rel":"sitemap",
         "data":[
          "name":"check",
          "value":""]}
        ]
    }

