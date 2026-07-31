# Firewall Rule Matrix

| Source | Destination | Port | Action | Purpose |
|----------|----------|----------|----------|----------|
| Any | WAF01 | 80 | Allow | HTTP Access |
| Any | WAF01 | 443 | Allow | HTTPS Access |
| Any | WEB01 | Any | Block | Prevent Direct Access |
| WAF01 | WEB01 | 80 | Allow | Forward Web Requests |
| WAF01 | WEB01 | 443 | Allow | Secure Forwarding |
| WAF01 | DC01 | 53 TCP/UDP | Allow | DNS Resolution |
| WAF01 | Splunk | 9997 | Allow | Log Forwarding |
| Kali Linux | WAF01 | 80/443 | Allow | Security Testing |
