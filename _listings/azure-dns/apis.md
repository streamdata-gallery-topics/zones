---
name: Azure DNS
x-slug: azure-dns
description: Azure DNS lets you host your DNS domains alongside your Azure apps and
  manage DNS records by using your existing Azure subscription. Microsoft&rsquo;s
  global network of name servers has the reach, scale, and redundancy to ensure ultra-fast
  DNS responses and ultra-high availability for your domains. With Azure DNS, you
  can be sure your DNS will always be fast and available.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-dns-01-host.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Zones
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/azure-dns/apis.md
specificationVersion: "0.14"
apis:
- name: Azure DNS API Zones Create Or Update
  x-api-slug: azure-dns-api
  description: Creates or updates a DNS zone. Does not modify DNS records within the
    zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-dns-01-host.png
  humanURL: https://azure.microsoft.com/en-us/services/dns/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}
  tags: Zones
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/azure-dns/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkdnszoneszonename-put-openapi.md
- name: Azure DNS API Zones Delete
  x-api-slug: azure-dns-api
  description: 'Deletes a DNS zone. WARNING: All DNS records in the zone will also
    be deleted. This operation cannot be undone.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-dns-01-host.png
  humanURL: https://azure.microsoft.com/en-us/services/dns/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}
  tags: Zones
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/azure-dns/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkdnszoneszonename-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/azure-dns/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkdnszoneszonename-delete-openapi.md
- name: Azure DNS API Zones Get
  x-api-slug: azure-dns-api
  description: Gets a DNS zone. Retrieves the zone properties, but not the record
    sets within the zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-dns-01-host.png
  humanURL: https://azure.microsoft.com/en-us/services/dns/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}
  tags: Zones
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/azure-dns/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkdnszoneszonename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/azure-dns/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkdnszoneszonename-get-openapi.md
- name: Azure DNS API Zones List By Resource Group
  x-api-slug: azure-dns-api
  description: Lists the DNS zones within a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-dns-01-host.png
  humanURL: https://azure.microsoft.com/en-us/services/dns/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones
  tags: Zones Resource Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/azure-dns/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkdnszones-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/azure-dns/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkdnszones-get-openapi.md
- name: Azure DNS API Zones List
  x-api-slug: azure-dns-api
  description: Lists the DNS zones in all resource groups in a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-dns-01-host.png
  humanURL: https://azure.microsoft.com/en-us/services/dns/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Network/dnszones
  tags: Zones
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/azure-dns/subscriptionssubscriptionidprovidersmicrosoft-networkdnszones-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/azure-dns/subscriptionssubscriptionidprovidersmicrosoft-networkdnszones-get-openapi.md
- name: Azure DNS API
  x-api-slug: azure-dns-api
  description: Azure DNS lets you host your DNS domains alongside your Azure apps
    and manage DNS records by using your existing Azure subscription. Microsoft&rsquo;s
    global network of name servers has the reach, scale, and redundancy to ensure
    ultra-fast DNS responses and ultra-high availability for your domains. With Azure
    DNS, you can be sure your DNS will always be fast and available.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-dns-01-host.png
  humanURL: https://azure.microsoft.com/en-us/services/dns/
  baseURL: ://management.azure.com//
  tags: Zones
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/zones/master/_listings/azure-dns/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/dns/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/dns/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/dns/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/dns/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---