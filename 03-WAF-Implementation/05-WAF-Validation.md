# WAF Validation

## XSS Test

Payload:

<script>alert(1)</script>

Expected Result:

403 Forbidden

Actual Result:

403 Forbidden

Status:

PASS

---

## SQL Injection Test

Payload:

' OR 1=1--

Expected Result:

403 Forbidden

Actual Result:

403 Forbidden

Status:

PASS

---

## ModSecurity Logging

Verified:

Yes

Evidence:

ModSecurity Access Denied Events

Status:

PASS

---

## Path Traversal

Payload:

../../../../etc/passwd

Expected Result:

Blocked

Actual Result:

400/404

Status:

PASS (Request unsuccessful)
