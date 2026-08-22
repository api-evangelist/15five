# 15Five (15five)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

15Five is a continuous performance management platform that helps organizations manage employee check-ins, OKRs, 1-on-1 meetings, pulse surveys, and manager effectiveness data. The platform provides a public REST API enabling IT admins and developers to build custom integrations that read and modify 15Five account data programmatically. Over 3,500 companies including Credit Karma, HubSpot, and Pendo rely on 15Five daily for performance and engagement management.

APIs.json: https://raw.githubusercontent.com/api-evangelist/15five/refs/heads/main/apis.yml

Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=15five-api-evangelist&utm_content=repo

## Tags

- Performance Management
- Employee Engagement
- OKRs
- Check-ins
- HR
- Human Resources
- 1-on-1 Meetings
- Pulse Surveys

## APIs

### 15Five Public API

RESTful API for reading and modifying 15Five account data including users, groups, objectives (OKRs), check-ins, review cycles, and performance data. Authentication uses API keys via HTTP Basic Auth. Rate-limited to 5 requests per second per IP address.

- Documentation: https://my.15five.com/api/public/
- Help Article: https://success.15five.com/hc/en-us/articles/50988142563483-15Five-Public-API-Supported-Features-Limits-and-Access-Rules

## Plans, Rate Limits, and FinOps

### Plans

15Five offers three core subscription tiers billed annually per user per month:

| Plan | Price |
|---|---|
| Engage | $4/user/month |
| Perform | $11/user/month |
| Total Platform | $16/user/month |

Add-ons include Kona Meeting Assistant ($2/employee/month), Kona Coach ($19/manager/month), Manager Content ($49/manager/month), Manager Coaching ($399/credit), and Compensation packages ($9–$11/user/month).

Full details: [plans/15five-plans-pricing.yml](plans/15five-plans-pricing.yml)

### Rate Limits

The 15Five API is rate-limited to **5 requests per second per IP address**. Exceeding this limit causes requests to be dropped with a 429 response; API keys are not suspended for rate limit violations.

Full details: [rate-limits/15five-rate-limits.yml](rate-limits/15five-rate-limits.yml)

### FinOps

15Five uses a per-user per-month subscription model (billed annually). Costs scale linearly with headcount. Finance teams can forecast spend by multiplying active user count by the per-user rate for each plan tier plus any applicable add-on charges.

Full details: [finops/15five-finops.yml](finops/15five-finops.yml)

## Timestamps

- Created: 2026-06-12
- Modified: 2026-06-12

## Common Properties

| Type | URL |
|---|---|
| Website | https://www.15five.com/ |
| Documentation | https://my.15five.com/api/public/ |
| Help Center | https://success.15five.com/hc/en-us/articles/360002699631-API |
| GitHub Organization | https://github.com/15five |
| LinkedIn | https://www.linkedin.com/company/15five |
| X | https://x.com/15Five |
| Blog | https://www.15five.com/blog |
| Pricing | https://www.15five.com/pricing |
| Status Page | https://status.15five.com/ |

## Maintainers

- Kin Lane / kin@apievangelist.com
