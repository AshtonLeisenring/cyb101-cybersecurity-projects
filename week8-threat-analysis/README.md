# Week 8 – Threat analysis with OSINT

Summary
Queried Shodan InternetDB for selected hosts, listed exposed ports and any CVEs, and looked up CVE details on NVD.

Tools used
curl, jq (optional), NVD website

Hosts analyzed
List at least five domains and their resolved IPs

Workflow
1) Resolve host to IP
2) Query InternetDB
   curl https://internetdb.shodan.io/<ip>
3) Note any vulns values and look them up on NVD
4) Summarize risk and likelihood in plain language

Example snippet
curl https://internetdb.shodan.io/1.2.3.4
# parse vulns and ports

Screenshots
Place here: screenshots/internetdb.png and screenshots/nvd.png

Ethics
Only analyze public OSINT and do not attempt to exploit anything
