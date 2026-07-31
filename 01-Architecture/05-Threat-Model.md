
# Threat Model

## SQL Injection

Attack Example:

```sql
' OR 1=1--
```

Impact:

- Authentication Bypass
- Database Access

Mitigation:

- ModSecurity
- OWASP CRS

---

## Cross Site Scripting

Attack Example:

```html
<script>alert(1)</script>
```

Impact:

- Session Theft
- Credential Theft

Mitigation:

- ModSecurity
- Input Validation

---

## Credential Stuffing

Tool:

```text
Hydra
```

Impact:

- Account Compromise

Mitigation:

- Rate Limiting
- Monitoring
- Account Lockout

---

## Path Traversal

Example:

```text
../../../../etc/passwd
```

Impact:

- File Disclosure

Mitigation:

- ModSecurity Rules

---

## HTTP Flood

Tools:

- ApacheBench
- Siege

Impact:

- Resource Exhaustion

Mitigation:

- Nginx Rate Limiting
- pfSense Filtering

---

## Reconnaissance

Tools:

- Nmap
- Nikto

Impact:

- Information Gathering

Mitigation:

- Firewall Restrictions
- Logging
- Monitoring
