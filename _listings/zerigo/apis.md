---
name: Zerigo
x-slug: zerigo
description: Zerigo makes DNS worry-free. With a REST API, user-friendly interface,
  and industry-leading advanced security and features, Zerigo DNS makes DNS easy and
  efficient.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/zerigo-logo.png
x-kinRank: "8"
x-alexaRank: ""
tags: Zones
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/apis.md
specificationVersion: "0.14"
apis:
- name: Zerigo List all zones
  x-api-slug: zerigo
  description: 'There are two optional parameters: page=# and per_page=#. page defaults
    to 1 (and starts at 1, not 0). per_page defaults to 100 but should be specified
    exactly if a change of the default value will cause your application to fail.
    The maximum value for per_page is 1000.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/zerigo-logo.png
  humanURL: https://www.zerigo.com
  baseURL: https://///api/1.1/zones.xml
  tags: Zones
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/api11zonesxml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/api11zonesxml-get-openapi.md
- name: Zerigo Count all zones
  x-api-slug: zerigo
  description: This is the total number of zones available. It is the same value as
    provided in the X-Query-Count header in the Managed DNS &#8594; List all zones
    API method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/zerigo-logo.png
  humanURL: https://www.zerigo.com
  baseURL: https:////header
  tags: Zones
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/header-xquerycount-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/header-xquerycount-openapi.md
- name: Zerigo Get a zone
  x-api-slug: zerigo
  description: This response is similar to Listing All Zones, with the addition of
    hosts-count and possibly hosts. As long as there are no more than 300 hosts, they
    will be returned. If there are more, the hosts array will be left out. hosts-count
    will always be returned.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/zerigo-logo.png
  humanURL: https://www.zerigo.com
  baseURL: https:////and
  tags: Zones
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/and-hostscount-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/and-hostscount-openapi.md
- name: Zerigo Get stats for a zone
  x-api-slug: zerigo
  description: This response returns current traffic statistics about this zone. Queries
    is measured from the beginning of the current period through the time of the API
    call. Just like everywhere else in our system, dates are based on UTC.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/zerigo-logo.png
  humanURL: https://www.zerigo.com
  baseURL: https://///api/1.1/zones/12345678/stats.xml
  tags: Zones
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/api11zones12345678statsxml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/api11zones12345678statsxml-get-openapi.md
- name: Zerigo Get a blank zone
  x-api-slug: zerigo
  description: This response may be useful to obtain a blank zone, suitable for use
    as a template or retrieving default values for included fields.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/zerigo-logo.png
  humanURL: https://www.zerigo.com
  baseURL: https://///api/1.1/zones/new.xml
  tags: Zones
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/api11zonesnewxml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/api11zonesnewxml-get-openapi.md
- name: Zerigo Create a zone
  x-api-slug: zerigo
  description: ns1 should be left out unless ns-type is &#8216;sec&#8217;. slave-nameservers
    should be left out unless ns-type is &#8216;pri&#8217;. See more details under
    Zones Overview.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/zerigo-logo.png
  humanURL: https://www.zerigo.com
  baseURL: https://///api/1.1/zones.xml
  tags: Zones
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/api11zonesxml-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/api11zonesxml-post-openapi.md
- name: Zerigo Update a zone
  x-api-slug: zerigo
  description: ns1 should be left out unless ns-type is &#8216;sec&#8217;. slave-nameservers
    should be left out unless ns-type is &#8216;pri&#8217;. See more details under
    Zones Overview.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/zerigo-logo.png
  humanURL: https://www.zerigo.com
  baseURL: https://///api/1.1/zones/12345678.xml
  tags: Zones
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/api11zones12345678xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/api11zones12345678xml-put-openapi.md
- name: Zerigo Delete a zone
  x-api-slug: zerigo
  description: Status 200 on success.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/zerigo-logo.png
  humanURL: https://www.zerigo.com
  baseURL: https://///api/1.1/zones/12345678.xml
  tags: Zones
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/api11zones12345678xml-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/api11zones12345678xml-delete-openapi.md
- name: Zerigo
  x-api-slug: zerigo
  description: Zerigo makes DNS worry-free. With a REST API, user-friendly interface,
    and industry-leading advanced security and features, Zerigo DNS makes DNS easy
    and efficient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/zerigo-logo.png
  humanURL: https://www.zerigo.com
  baseURL: https:///
  tags: Zones
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/zerigo/openapi.md
x-common:
- type: x-blog
  url: https://www.zerigo.com/blog
- type: x-blog-rss
  url: http://www.zerigo.com/blog.xml
- type: x-github
  url: https://github.com/zerigo
- type: x-status
  url: http://zerigostatus.com/
- type: x-twitter
  url: https://twitter.com/zerigo
- type: x-website
  url: https://www.zerigo.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---