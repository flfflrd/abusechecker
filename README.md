# abusechecker
A bash script to check and block abusive IPs


I wrote this program for my web server because i noticed a variety of unknown IPs trying to gain access through PHP vulnerabilities and web-cgi.
I dont know anything about security hardening in that regard so Ive written a simple script that checks each IP against abuseipdb.com's databases and stores their scores on a local db.
The program also has options to automatically block any IP with a score of 100, or confirmed abusive.
Its a pretty janky work but it was fun to make
