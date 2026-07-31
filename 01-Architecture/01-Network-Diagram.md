# Atlas Financial Group Network Diagram

## Architecture

```text
                    Internet
                        |
                        |
                  pfSense Firewall
                        |
              Port Forward 80/443
                        |
                 ----------------
                 |              |
               WAF01      Splunk Logs
           (10.10.30.5)
                 |
                 |
               WEB01
          (10.10.30.10)
                 |
          ----------------
          |              |
        DC01          Splunk
```

## Traffic Flow

User
→ Internet
→ pfSense
→ WAF01
→ WEB01

Direct access to WEB01 is prohibited.

## Security Boundary

Internet-facing systems:

- WAF01
- WEB01

Internal infrastructure:

- DC01
- FS01
- Splunk
- OpenVAS

Management systems:

- Kali Linux
- Admin Workstation
