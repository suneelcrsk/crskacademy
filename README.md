crsk.academy — static site

This folder contains the landing page for crsk.academy. It is a simple static site (index.html + styles.css).

Next steps to deploy to GitHub + Netlify

1) Create a GitHub repo (on your GitHub account) called crskacademy or similar.

2) From the workspace run (replace <your-repo-url>):

   cd /Users/crsk/.openclaw/workspace/site
   git init
   git add .
   git commit -m "initial site"
   git remote add origin https://github.com/suneelcrsk/crskacademy.git
   git branch -M main
   git push -u origin main

3) On Netlify:
   - Log in to your Netlify account and go to Sites → New site from Git → GitHub
   - Authorize Netlify to access your repo (if not already). Select the crskacademy repo and deploy.
   - In Site settings → Domain management, add custom domain crsk.academy.
   - Netlify will provide DNS records (A/CNAME) or an option to update nameservers. Copy the DNS instructions.

4) In your Spaceship domain control panel, add the DNS records Netlify provided to point crsk.academy to Netlify.

5) Once DNS propagates, Netlify will issue TLS and the site will be live.

If you want me to complete the Netlify deploy for you while you authorize Netlify to access GitHub, I can guide you interactively — tell me when you're ready and I will provide the exact clicks and settings.
