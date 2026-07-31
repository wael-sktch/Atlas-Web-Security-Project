# IP Addressing Plan

## User Network

Network:

```text
10.10.10.0/24
```

Purpose:

Employee Workstations

Systems:

- USER-PC1
- USER-PC2
- USER-PC3

---

## Server Network

Network:

```text
10.10.20.0/24
```

Purpose:

Infrastructure Services

Systems:

- DC01
- FS01
- Splunk
- OpenVAS

---

## DMZ Network

Network:

```text
10.10.30.0/24
```

Purpose:

Internet-facing Systems

Systems:

- WAF01 (10.10.30.5)
- WEB01 (10.10.30.10)

---

## Management Network

Network:

```text
10.10.40.0/24
```

Purpose:

Administration and Security Testing

Systems:

- Kali Linux
- Admin Workstation
