FUTURE_CS_03
Project Overview

This project focuses on performing a read-only API Security Risk Analysis on a public demo API. Modern web applications, mobile apps, SaaS platforms, and dashboards rely heavily on APIs for communication and data exchange.

The objective of this task is to analyze API responses, review authentication controls, inspect headers, and identify common security risks without exploiting or attacking the system.

---

API Selected for Testing

JSONPlaceholder

Base URL:

https://jsonplaceholder.typicode.com

Endpoint Tested:

https://jsonplaceholder.typicode.com/users

---

Scope of Testing

This assessment was conducted under ethical and safe boundaries.

Included

- Public API endpoint review
- Read-only GET requests
- Response data inspection
- Header review
- Authentication check
- Risk analysis

Excluded

- Exploitation attempts
- Authentication bypass
- DoS / flooding
- Private system access
- Destructive testing

---

Tools Used

- Postman
- Browser Developer Tools
- Markdown Documentation
- GitHub

---

Testing Methodology

1. Selected a safe public demo API.
2. Sent GET requests using Postman.
3. Verified server responses.
4. Reviewed returned JSON data.
5. Checked whether authentication was required.
6. Identified security risks.
7. Classified severity levels.
8. Prepared remediation recommendations.

---

Key Findings

Finding| Severity| Description
Unauthenticated Access| Medium| Endpoint returned data without login or token.
Excessive Data Exposure| Medium| API response included phone, website, and company details.
Predictable Resource Access| Low| Public numeric IDs may allow easy enumeration.
Missing Rate Limiting Evidence| Low| No visible throttling controls on demo endpoint.

---

Business Impact

- Public exposure of user metadata can support phishing or spam campaigns.
- Lack of authentication may allow unrestricted data scraping.
- Predictable IDs may help attackers collect bulk records.
- Weak API controls reduce trust in SaaS platforms.

---

Security Recommendations

1. Require authentication for user-related endpoints.
2. Return only necessary fields in responses.
3. Implement role-based access control.
4. Add API rate limiting and abuse detection.
5. Use secure headers and token validation.
6. Monitor logs for unusual request activity.

---

Evidence

Screenshots of Postman requests and responses are available in the "/screenshots" folder.

---

Repository Structure

api-security-risk-analysis/
│── README.md
│── report.pdf
│── screenshots/
│   └── api-response.png

---

Learning Outcome

Through this project, I gained practical knowledge in:

- API testing
- Security risk identification
- Authentication review
- OWASP API risk awareness
- Professional reporting

---

Disclaimer

This project was performed only on a public demo API intended for learning and testing. No unauthorized activity was conducted.

