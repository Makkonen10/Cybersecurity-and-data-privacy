About This Report
Report Parameters
Contexts
No contexts were selected, so all contexts were included by default.

Sites
The following sites were included:

http://localhost:8001
(If no sites were selected, all sites were included by default.)

An included site must also be within one of the included contexts for its data to be included in the report.

Risk levels
Included: High, Medium, Low, Informational

Excluded: None

Confidence levels
Included: User Confirmed, High, Medium, Low

Excluded: User Confirmed, High, Medium, Low, False Positive

Summaries
Alert Counts by Risk and Confidence
This table shows the number of alerts for each level of risk and confidence included in the report.

(The percentages in brackets represent the count as a percentage of the total number of alerts included in the report, rounded to one decimal place.)

Confidence
User Confirmed	High	Medium	Low	Total
Risk	High	0
(0.0%)	0
(0.0%)	0
(0.0%)	0
(0.0%)	0
(0.0%)
Medium	0
(0.0%)	1
(20.0%)	1
(20.0%)	1
(20.0%)	3
(60.0%)
Low	0
(0.0%)	0
(0.0%)	2
(40.0%)	0
(0.0%)	2
(40.0%)
Informational	0
(0.0%)	0
(0.0%)	0
(0.0%)	0
(0.0%)	0
(0.0%)
Total	0
(0.0%)	1
(20.0%)	3
(60.0%)	1
(20.0%)	5
(100%)
Alert Counts by Site and Risk
This table shows, for each site for which one or more alerts were raised, the number of alerts raised at each risk level.

Alerts with a confidence level of "False Positive" have been excluded from these counts.

(The numbers in brackets are the number of alerts raised for the site at or above that risk level.)

Risk
High
(= High)	Medium
(>= Medium)	Low
(>= Low)	Informational
(>= Informational)
Site	http://localhost:8001	0
(0)	3
(3)	2
(5)	0
(5)
Alert Counts by Alert Type
This table shows the number of alerts of each alert type, together with the alert type's risk level.

(The percentages in brackets represent each count as a percentage, rounded to one decimal place, of the total number of alerts included in this report.)

Alert type	Risk	Count
Absence of Anti-CSRF Tokens	Medium	1
(20.0%)
Content Security Policy (CSP) Header Not Set	Medium	2
(40.0%)
Missing Anti-clickjacking Header	Medium	2
(40.0%)
Application Error Disclosure	Low	1
(20.0%)
X-Content-Type-Options Header Missing	Low	5
(100.0%)
Total		5
Insights
This table shows information that is likely to be very relevant to you, but which is not related to vulnerabilities, or potentially even related to the application in question.

Level	Reason	Site	Description	Statistic
Low
Warning
ZAP errors logged - see the zap.log file for details
1
Info
Informational
http://localhost:8001
Percentage of responses with status code 2xx
40 %
Info
Informational
http://localhost:8001
Percentage of responses with status code 3xx
1 %
Info
Informational
http://localhost:8001
Percentage of responses with status code 4xx
58 %
Info
Informational
http://localhost:8001
Percentage of endpoints with content type text/css
9 %
Info
Informational
http://localhost:8001
Percentage of endpoints with content type text/html
18 %
Info
Informational
http://localhost:8001
Percentage of endpoints with content type text/javascript
18 %
Info
Informational
http://localhost:8001
Percentage of endpoints with content type text/plain
45 %
Info
Informational
http://localhost:8001
Percentage of endpoints with method GET
90 %
Info
Informational
http://localhost:8001
Percentage of endpoints with method POST
9 %
Info
Informational
http://localhost:8001
Count of total endpoints
11
Alerts
Risk=Medium, Confidence=High (1)
http://localhost:8001 (1)
Content Security Policy (CSP) Header Not Set (1)
GET http://localhost:8001/
Risk=Medium, Confidence=Medium (1)
http://localhost:8001 (1)
Missing Anti-clickjacking Header (1)
GET http://localhost:8001/
Risk=Medium, Confidence=Low (1)
http://localhost:8001 (1)
Absence of Anti-CSRF Tokens (1)
GET http://localhost:8001/register
Risk=Low, Confidence=Medium (2)
http://localhost:8001 (2)
Application Error Disclosure (1)
POST http://localhost:8001/register
X-Content-Type-Options Header Missing (1)
GET http://localhost:8001/static/footer.js
Appendix
Alert Types
This section contains additional information on the types of alerts in the report.

Absence of Anti-CSRF Tokens
Source	raised by a passive scanner (Absence of Anti-CSRF Tokens)
CWE ID	352
WASC ID	9
Reference	
https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html
https://cwe.mitre.org/data/definitions/352.html
Content Security Policy (CSP) Header Not Set
Source	raised by a passive scanner (Content Security Policy (CSP) Header Not Set)
CWE ID	693
WASC ID	15
Reference	
https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/CSP
https://cheatsheetseries.owasp.org/cheatsheets/Content_Security_Policy_Cheat_Sheet.html
https://www.w3.org/TR/CSP/
https://w3c.github.io/webappsec-csp/
https://web.dev/articles/csp
https://caniuse.com/#feat=contentsecuritypolicy
https://content-security-policy.com/
Missing Anti-clickjacking Header
Source	raised by a passive scanner (Anti-clickjacking Header)
CWE ID	1021
WASC ID	15
Reference	
https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/X-Frame-Options
Application Error Disclosure
Source	raised by a passive scanner (Application Error Disclosure)
CWE ID	550
WASC ID	13
X-Content-Type-Options Header Missing
Source	raised by a passive scanner (X-Content-Type-Options Header Missing)
CWE ID	693
WASC ID	15
Reference	
https://learn.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/compatibility/gg622941(v=vs.85)
https://owasp.org/www-community/Security_Headers
