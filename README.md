# Onedrive-proxy-workers
A simple script that runs on Cloudflare Workers to speed up downloading of Onedrive for Business files and avoid Cloudflare account bans  

# How does it works?  
If the reverse proxy target is not a file, the script will not proxy and return 403, which effectively avoids being banned by Cloudflare on the grounds of phishing websites.  

# How to use?  
Copy all the contents in index.js, paste it into the Workers code editor, modify the original reverse address to your own onedrive for Business subdomain (the format is xxxxxx-my.sharepoint.com), and then save the deployment. Bind the custom domain, and then fill in the reverse domain name where needed (such as Alist, onemanger).
