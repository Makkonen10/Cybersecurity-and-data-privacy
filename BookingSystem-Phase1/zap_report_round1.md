***

# ⚡ ZAP Security Scan Report 

## **About This Report**

### **Report Parameters**

**Contexts**  
No contexts were selected, so all contexts were included by default.

**Sites Included**

*   <http://localhost:8001>  
    (If no sites were selected, all were included.)

> *A site must also be within one of the included contexts for its data to be included.*

**Risk Levels**

*   **Included:** High, Medium, Low, Informational
*   **Excluded:** None

**Confidence Levels**

*   **Included:** User Confirmed, High, Medium, Low
*   **Excluded:** User Confirmed, High, Medium, Low, False Positive

***

## **Summaries**

### **Alert Counts by Risk and Confidence**

| Risk          | User Confirmed | High      | Medium    | Low       | Total        |
| ------------- | -------------- | --------- | --------- | --------- | ------------ |
| High          | 0 (0.0%)       | 0 (0.0%)  | 0 (0.0%)  | 0 (0.0%)  | 0 (0.0%)     |
| Medium        | 0 (0.0%)       | 1 (20.0%) | 1 (20.0%) | 1 (20.0%) | 3 (60.0%)    |
| Low           | 0 (0.0%)       | 0 (0.0%)  | 2 (40.0%) | 0 (0.0%)  | 2 (40.0%)    |
| Informational | 0 (0.0%)       | 0 (0.0%)  | 0 (0.0%)  | 0 (0.0%)  | 0 (0.0%)     |
| **Total**     | 0 (0.0%)       | 1 (20.0%) | 3 (60.0%) | 1 (20.0%) | **5 (100%)** |

***

### **Alert Counts by Site and Risk**

| Site                    | High (≥High) | Medium (≥Medium) | Low (≥Low) | Informational (≥Informational) |
| ----------------------- | ------------ | ---------------- | ---------- | ------------------------------ |
| <http://localhost:8001> | 0 (0)        | 3 (3)            | 2 (5)      | 0 (5)                          |

***

### **Alert Counts by Alert Type**

| Alert Type                                   | Risk   | Count     |
| -------------------------------------------- | ------ | --------- |
| Absence of Anti-CSRF Tokens                  | Medium | 1 (20.0%) |
| Content Security Policy (CSP) Header Not Set | Medium | 2 (40.0%) |
| Missing Anti-clickjacking Header             | Medium | 2 (40.0%) |
| Application Error Disclosure                 | Low    | 1 (20.0%) |
| X-Content-Type-Options Header Missing        | Low    | 5 (100%)  |
| **Total**                                    | —      | **5**     |

***

## **Insights**

| Level | Reason        | Site                    | Description                     | Statistic |
| ----- | ------------- | ----------------------- | ------------------------------- | --------- |
| Low   | Warning       | —                       | ZAP errors logged – see zap.log | 1         |
| Info  | Informational | <http://localhost:8001> | % responses status 2xx          | 40%       |
| Info  | Informational | <http://localhost:8001> | % responses status 3xx          | 1%        |
| Info  | Informational | <http://localhost:8001> | % responses status 4xx          | 58%       |
| Info  | Informational | <http://localhost:8001> | % endpoints text/css            | 9%        |
| Info  | Informational | <http://localhost:8001> | % endpoints text/html           | 18%       |
| Info  | Informational | <http://localhost:8001> | % endpoints text/javascript     | 18%       |
| Info  | Informational | <http://localhost:8001> | % endpoints text/plain          | 45%       |
| Info  | Informational | <http://localhost:8001> | % endpoints GET                 | 90%       |
| Info  | Informational | <http://localhost:8001> | % endpoints POST                | 9%        |
| Info  | Informational | <http://localhost:8001> | Total endpoints                 | 11        |

***

## **Alerts**

### **Medium Risk, High Confidence (1)**

**Site:** <http://localhost:8001>

*   **Content Security Policy (CSP) Header Not Set**
    *   GET <http://localhost:8001/>

***

### **Medium Risk, Medium Confidence (1)**

**Site:** <http://localhost:8001>

*   **Missing Anti-clickjacking Header**
    *   GET <http://localhost:8001/>

***

### **Medium Risk, Low Confidence (1)**

**Site:** <http://localhost:8001>

*   **Absence of Anti-CSRF Tokens**
    *   GET <http://localhost:8001/register>

***

### **Low Risk, Medium Confidence (2)**

**Site:** <http://localhost:8001>

*   **Application Error Disclosure**
    *   POST <http://localhost:8001/register>
*   **X-Content-Type-Options Header Missing**
    *   GET <http://localhost:8001/static/footer.js>

***

## **Appendix: Alert Types**

### **Absence of Anti-CSRF Tokens**

*   **Source:** Passive scanner
*   **CWE:** 352
*   **WASC:** 9
*   **References:**
    *   <https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html>
    *   <https://cwe.mitre.org/data/definitions/352.html>

### **Content Security Policy (CSP) Header Not Set**

*   **Source:** Passive scanner
*   **CWE:** 693
*   **WASC:** 15
*   **References:**
    *   <https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/CSP>
    *   <https://cheatsheetseries.owasp.org/cheatsheets/Content_Security_Policy_Cheat_Sheet.html>
    *   <https://www.w3.org/TR/CSP/>

### **Missing Anti-clickjacking Header**

*   **Source:** Passive scanner
*   **CWE:** 1021
*   **WASC:** 15
*   **Reference:** <https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/X-Frame-Options>

### **Application Error Disclosure**

*   **Source:** Passive scanner
*   **CWE:** 550
*   **WASC:** 13

### **X-Content-Type-Options Header Missing**

*   **Source:** Passive scanner
*   **CWE:** 693
*   **WASC:** 15
*   **References:**
    *   <https://learn.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/compatibility/gg622941(v=vs.85)>
    *   <https://owasp.org/www-community/Security_Headers>

***


