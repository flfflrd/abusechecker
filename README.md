# abusechecker

### A bash script to check and block abusive IPs
This program depends upon sqlite3 and jq and ufw




#### 2023 update
Updated to be quickly usable on a new machine, debian-based in particular.\
I lost the schema for the database but Sithum said chatgpt it, so theres an initDatabase program for that now\
The program now checks all previous logs, including the gzipped ones.\
-g output made more legible
- [ ] nslookup, and whois data will be added in future
- [ ] Gotta remove my personal API key...



I wrote this program for my web server because I noticed a variety of unknown IPs trying to gain access through PHP vulnerabilities and web-cgi.\
I dont know much about security hardening in that regard so I've written a simple script that checks each IP against abuseipdb.com's databases and stores their scores on a local db.\
The program also has options to automatically block any IP with a score of 100, or confirmed abusive.\
Its a pretty janky work but it was fun to make
