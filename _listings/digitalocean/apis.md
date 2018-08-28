---
name: DigitalOcean
x-slug: digitalocean
description: DigitalOcean is a simple and fast cloud hosting service built for developers.
  Customers can create a cloud server in 55 seconds, and pricing plans start at only
  $5 per month for 512MB of RAM, 20GB SSD, 1 CPU, and 1TB Transfer. Featuring a 99.99%
  Uptime SLA, DigitalOcean has servers located in New York, San Francisco, and Amsterdam.
  The DigitalOcean control panel interface is simple and intuitive, which power users
  can replicate on a larger scale with the company&rsquo;s API. DigitalOcean uses
  KVM virtualization and additionally hosts a library of helpful walkthroughs and
  tutorials that cover server configuration and optimization.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
x-kinRank: "7"
x-alexaRank: "0"
tags: New
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/digitalocean/apis.md
specificationVersion: "0.14"
apis:
- name: DigitalOcean API-V2 - Create a new certificate
  x-api-slug: certificates-post
  description: To upload or create a new SSL certificate, send a POST request to /v2/certificates.
    When uploading a user-generated certificate, the private_key, leaf_certificate,
    and optionally the certificate_chain attributes should be provided. The type should
    be set to "custom". When generating a certificate using Let's Encrypt, the dns_names
    attribute must be provided, and the type should be set to "lets_encrypt".
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/digitalocean/certificates-post-openapi.md
- name: DigitalOcean API-V2 - Create a new Droplet
  x-api-slug: droplets-post
  description: To create a new Droplet, send a POST request to /v2/droplets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/digitalocean/droplets-post-openapi.md
- name: DigitalOcean API-V2 - Create a new Key
  x-api-slug: accountkeys-post
  description: "To add a new SSH public key to your DigitalOcean account, send a POST
    request to /v2/account/keys. Set the \"name\" attribute to the name you wish to
    use and the \"public_key\" attribute to a string of the full public key you are
    adding.\n\nThe response body will be a JSON object with a key set to ssh_key.
    The value will be the complete generated key object. This will have the standard
    key attributes:\n\nName\tType\tDescription\nid\tinteger\tThis is a unique identification
    number for the key. This can be used to reference a specific SSH key when you
    wish to embed a key into a Droplet.\nfingerprint\tstring\tThis attribute contains
    the fingerprint value that is generated from the public key. This is a unique
    identifier that will differentiate it from other keys using a format that SSH
    recognizes.\npublic_key\tstring\tThis attribute contains the entire public key
    string that was uploaded. This is what is embedded into the root user's authorized_keys
    file if you choose to include this SSH key during Droplet creation.\nname\tstring\tThis
    is the human-readable display name for the given SSH key. This is used to easily
    identify the SSH keys when they are displayed."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/digitalocean/accountkeys-post-openapi.md
- name: DigitalOcean API-V2 - Create a new Tag
  x-api-slug: tags-post
  description: "To create a Tag you can send a POST request to /v2/tags with a name
    attribute.\r\n\r\nThe response will be a JSON object with a key called _tag_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/digitalocean/tags-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://digital.river.api.gallery.streamdata.io
- type: x-api-stack
  url: http://digitalocean.stack.network
- type: x-base
  url: https://api.digitalocean.com/
- type: x-blog
  url: https://www.digitalocean.com/company/blog/
- type: x-blog-rss
  url: https://www.digitalocean.com/company/blog/feed.xml
- type: x-command-line-interface
  url: https://github.com/digitalocean/doctl
- type: x-developer
  url: https://developers.digitalocean.com/
- type: x-github
  url: https://github.com/digitalocean
- type: x-twitter
  url: https://twitter.com/digitalocean
- type: x-website
  url: https://www.digitalocean.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---