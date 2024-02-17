# Onedrive-proxy-workers
A simple script that runs on Cloudflare Workers to speed up downloading of Onedrive for Business files and avoid Cloudflare account bans
＃ How does it works?  
If the reverse proxy target is not a file, the script will not proxy and return 403, which effectively avoids being banned by Cloudflare on the grounds of phishing websites.
