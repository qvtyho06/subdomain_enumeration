## Project Overview

### How it works (an analogy)
Think of `example.com` as a neighborhood. You know the neighborhood's name, but not which houses are in it. This tool takes a list of common house names like "www", "mail", "admin", "dev" and "shop". For each one, it asks the post office (a DNS server): "Does `admin.example.com` exist, and what is its address?" If the post office gives an address, the tool writes it down. If not, it moves on to the next name. It can also check public records, such as SSL certificate logs and search engines, to find houses without knocking at all.

### Input
- A root domain, e.g. `example.com`
- A wordlist of candidate subdomain names
- Optional settings, such as the number of concurrent threads

### Output
- A list of live subdomains with their IP addresses, e.g. `mail.example.com -> 203.0.113.5`
- Results can be saved as TXT, CSV or JSON

### Real-world use
Security professionals use subdomain enumeration during reconnaissance, the first phase of penetration testing and bug bounty work. It maps an organization's internet-facing attack surface. It often reveals forgotten admin panels, unpatched staging servers, or abandoned subdomains that are open to takeover. Defenders run it on their own domains to find and fix these exposures first.

> **Disclaimer:** Only scan domains you own or have explicit permission to test.