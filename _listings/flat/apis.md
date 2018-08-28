---
name: Flat
x-slug: flat
description: Whether youre a beginner or a professional composer, our user-friendly
  music composition software gives you all the tools that you need to make your own
  sheet music. You can write, listen, share and discover music scores right in your
  web browser on any device
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: New
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/flat/apis.md
specificationVersion: "0.14"
apis:
- name: Flat - Create a new score
  x-api-slug: scores-post
  description: |-
    Use this API method to **create a new music score in the current User account**. You will need a MusicXML 3 (`vnd.recordare.musicxml` or `vnd.recordare.musicxml+xml`) or a MIDI (`audio/midi`) file to create the new Flat document.

    This API call will automatically create the first revision of the document, the score can be modified by the using our web application or by uploading a new revision of this file (`POST /v2/scores/{score}/revisions/{revision}`).

    The currently authenticated user will be granted owner of the file and will be able to add other collaborators (users and groups).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/flat/scores-post-openapi.md
- name: Flat - Add a new collaborator
  x-api-slug: scoresscorecollaborators-post
  description: |-
    Share a score with a single user or a group. This API call allows to add, invite and update the collaborators of a document.
    - To add an existing Flat user to the document, specify its unique identifier in the `user` property.
    - To invite an external user to the document, specify its email in the `userEmail` property.
    - To add a Flat group to the document, specify its unique identifier in the `group` property.
    - To update an existing collaborator, process the same request with different rights.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/flat/scoresscorecollaborators-post-openapi.md
- name: Flat - Post a new comment
  x-api-slug: scoresscorecomments-post
  description: |-
    Post a document or a contextualized comment on a document.

    Please note that this method includes an anti-spam system for public scores. We don't guarantee that your comments will be accepted and displayed to end-user. Comments are be blocked by returning a `403` HTTP error and hidden from other users when the `spam` property is `true`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/flat/scoresscorecomments-post-openapi.md
- name: Flat - Create a new revision
  x-api-slug: scoresscorerevisions-post
  description: Update a score by uploading a new revision for this one.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/new/master/_listings/flat/scoresscorerevisions-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://fitbit.api.gallery.streamdata.io
- type: x-api-stack
  url: http://flat.stack.network
- type: x-developer
  url: https://flat.io/developers
- type: x-embeddable
  url: https://flat.io/developers/embed
- type: x-github
  url: https://github.com/FlatIO
- type: x-pricing
  url: https://flat.io/pricing
- type: x-privacy-policy
  url: https://flat.io/help/en/policies/#coppa-and-ferpa-compliance
- type: x-support
  url: https://flat.io/help
- type: x-twitter
  url: https://twitter.com/flat_io
- type: x-website
  url: http://flat.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---