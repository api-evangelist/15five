# 15Five (15five)

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
