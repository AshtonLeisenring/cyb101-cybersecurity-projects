# Week 3 – Password cracking practice with John

Summary
Cracked a synthetic hash set using John the Ripper, explored wordlists, rules, and masks, and reported results.

Tools used
john, wordlists, masks, rules

Data
A 1000 entry hash file provided in class

Approach
- Started with a short wordlist to get baseline
- Switched to a larger wordlist
- Applied built in rule sets
- Tried a custom mask for short numeric or mixed length passwords

Commands I ran (examples only, adjust to what you actually used)
john --wordlist=/path/to/rockyou.txt cp_leak.txt
john --rules=Single --wordlist=... cp_leak.txt
john --mask='[a-z][a-z][a-z][a-z][0-9]' cp_leak.txt
john --show cp_leak.txt

Results
- Total cracked
- Fastest strategy
- Any interesting patterns

Screenshots
Place here: screenshots/john_progress.png and screenshots/john_show.png

Ethics
Only work on owned or explicitly authorized datasets
