swagger: "2.0"
x-collection-name: LiveChat
x-complete: 1
info:
  title: LiveChat REST API
  description: -introductionwelcome-to-the-livechat-api-documentationour-api-provides-a-set-of-flexible-tools-which-you-can-use-to-create-new-outstanding-projects--we-smile-a-bit-more-each-time-we-see-skilled-developers-unleash-their-creativityplease-note-that-this-documentation-refers-to-the-latest-api-version-2-0--if-you-are-looking-for-the-previous-version-check-out-the-deprecated-api-1-0-documentation--basic-api-usageall-livechat-api-requests-start-with--httpsapi-livechatinc-com-please-note-that-all-livechat-api-requests-must-use-https-protocol-the-next-segment-of-the-url-path-depends-on-the-type-of-your-request--for-example-use--httpsapi-livechatinc-comagents--to-get-or-modify-the-agents-data-all-requests-must-have-xapiversion-header-set-to-the-number-of-the-version-that-youd-like-to-use--the-most-recent-version-is-2--authenticationtwo-common-authentication-methods-are-supported--oauth-2-0--and--api-key--oauth-2-0oauth-2-0-authentication-is-the-recommended-way-of-authenticating-to-livechat-api-it-is-the-most-secure-way-of-making-api-calls--with-this-flow-you-will-get-access-only-to-some-parts-of-livechat-account-such-as-reading-agents-list--this-is-more-secure-than--api-key-flowhttpsdocs-livechatinc-comrestapiapikey--which-has-always-access-to-all-livechat-account-data-to-start-using-oauth-2-0-please-read-a-dedicated--authorizationhttpsdocs-livechatinc-comauthorization--guide--api-keyif-you-want-to-build-a-private-app-that-will-run-on-your-own-server-you-can-skip-the-oauth-2-0-flow-and-use-the-api-key--please-note-this-flow-of-making-api-calls-is-less-secure-because-the-api-key-gives-access-to-all-livechat-account-data-with-this-authorization-method-you-will-need-to-include-your-livechat-login-and--api-key--for-each-method-call--youll-find-the-api-key-in--your-livechat-profilehttpsmy-livechatinc-comagentsapikey-authentication-to-the-api-occurs-via--http-basic-authhttpen-wikipedia-orgwikibasic-access-authentication--provide-your--login--as-the-basic-auth-username-and-the--api-key--as-the-password--you-must-authenticate-for-all-requests-all-api-requests-must-be-made-over-https--data-formatthe-livechat-api-returns-the-data-in-the--jsonhttpen-wikipedia-orgwikijson--format--check-out-the-following-example--jsonpall-requests-made-with-http-get-are--jsonphttpen-wikipedia-orgwikijsonpenabled--to-use-jsonp-append--callback--and-the-name-of-your-callback-function-to-the-request--error-handlingthe-errors-are-returned-using-the-standard-http-error-code-syntax--in-general-the-codes-in-the-2xx-range-indicate-success-the-codes-in-the-4xx-range-indicate-an-error-incorrect-or-missing-parameters-not-authenticated-etc--and-the-codes-in-the-5xx-range-indicate-an-error-with-the-livechat-servers--any-additional-info-is-included-in-the-body-of-the-return-call-jsonformatted--http-status-codes-summary---400---the-request-is-incorrect-please-make-sure-that-the-passed-arguments-are-matching-the-format-in-the-methods-documentation----401---unauthorized--you-attempt-to-authenticate-with-an-invalid-username-or-api-key----404---not-found--you-attempt-to-request-a-resource-which-doesnt-exist----500---internal-server-error--something-unexpected-happened-on-our-end--please-try-again-or-contact-our-support--crossdomainall-crossdomain-api-requests-made-by-a-web-browser-are-denied-for-security-reasons--it-means-that-the-browserbased-requests-are-not-allowed-from-3rd-party-domains-including--localhost--livechat-api-librariesall-api-calls-include-an-api-key-that-can-be-easily-stolen-when-making-a-request-using-a-web-browser--it-means-you-should-use-backend-languages-for-api-requests--here-is-a-list-of-the-readytouse-libraries---php-library-for-livechat-apihttpsgithub-comlivechatapiclientphp-hosted-on-github----node-js-library-for-livechat-apihttpsgithub-comlivechatapiclientnodejs-hosted-on-github----ruby-library-for-livechat-apihttpsgithub-comcxzlivechat-client-hosted-on-github----c-library-for-livechat-apihttpsgithub-comlivechatapiclientcsharp-hosted-on-github--external-livechat-api-libraries---r-library-for-livechat-apihttpsgithub-comlawwulivechatr-hosted-on-github-did-you-write-your-own-library-and-want-it-listed-here-let-us-know
  version: 1.0.0
host: api.livechatinc.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/tickets/new_tickets:
    get:
      summary: New tickets
      description: Shows the number of the tickets created during the specified period.
      operationId: ReportsTicketsNewTicketsGet
      x-api-path-slug: reportsticketsnew-tickets-get
      parameters:
      - in: query
        name: date_from
      - in: query
        name: date_to
      - in: query
        name: group_by
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - New
      - Tickets
  /agents:
    post:
      summary: Create a new agent
      description: Creates a new agent in your license.
      operationId: AgentsPost
      x-api-path-slug: agents-post
      parameters:
      - in: formData
        name: login
      - in: formData
        name: name
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - New
      - Agent
  /goals:
    post:
      summary: Add a new goal
      description: Creates a new goal.
      operationId: GoalsPost
      x-api-path-slug: goals-post
      parameters:
      - in: formData
        name: match_type
      - in: formData
        name: name
      - in: formData
        name: type
      - in: formData
        name: url
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - New
      - Goal
  /groups:
    post:
      summary: Create a new group
      description: Creates a new group in your license.
      operationId: GroupsPost
      x-api-path-slug: groups-post
      parameters:
      - in: formData
        name: agents[0]
      - in: formData
        name: agents[1]
      - in: formData
        name: name
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - New
      - Group
  /canned_responses:
    post:
      summary: Create a new canned response
      description: Creates a new canned response.
      operationId: CannedResponsesPost
      x-api-path-slug: canned-responses-post
      parameters:
      - in: formData
        name: tags[0]
      - in: formData
        name: tags[1]
      - in: formData
        name: text
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - New
      - Canned
      - Response
  /webhooks:
    post:
      summary: Create a new webhook
      description: Creates a new webhook.
      operationId: WebhooksPost
      x-api-path-slug: webhooks-post
      parameters:
      - in: formData
        name: data_types[]
      - in: formData
        name: event_type
      - in: formData
        name: url
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - New
      - Webhook
  /greetings:
    post:
      summary: Create a new greeting
      description: Use this function to create a new greeting.
      operationId: GreetingsPost
      x-api-path-slug: greetings-post
      parameters:
      - in: formData
        name: name
      - in: formData
        name: rules[0][operator]
      - in: formData
        name: rules[0][type]
      - in: formData
        name: rules[0][value]
      - in: formData
        name: rules[1][operator]
      - in: formData
        name: rules[1][type]
      - in: formData
        name: rules[1][value]
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - New
      - Greeting