<!SLIDE lightblue-title padding-bottom>

# Create Media Types

<!SLIDE medium-paras>

Media type design is just as much an art as it is a science.

<!SLIDE lightblue-title media-definition>

# Needed in a definition:

* data elements
* hypermedia controls

<!SLIDE lightblue-title medium-paras padding-bottom>

# w3clove.validation+json
application/vnd.w3clove.validation+json

<!SLIDE lightblue-title>

# Data Elements

    {
      "created_at": "2012-01-30T01:17:04Z",
      "scraped_at": "2012-01-30T01:17:10Z",
      "scraping_success": true,
      "url": "http://www.zeldman.com",

<!SLIDE lightblue-title medium-paras>

# Data Elements

A response MAY contain `created_at`, `scraped_at`, `scraping_success`, `updated_at`, `url`, `web_pages_count`, `validation_errors_count`, `validation_warnings_count`, and `pending_count` elements.

<!SLIDE lightblue-title medium-paras>

# Hypermedia Controls

A response MAY include a `forms` element, which is an array of objects. They MUST have these elements: `href`, `rel`, and `data` elements. `data` will be an array of objects that MUST have two keys, `name`, and `value`.

<!SLIDE lightblue-title medium-paras>

# Hypermedia Controls

* `sitemap-form`: Following a link with this rel will lead you to a resource with a form for generating a Sitemap API request.
* `sitemap`: Processing a form with this rel will lead you to a resource that gives you validation information about a sitemap.
