# True Size — deploy guide
1. Replace `https://YOUR-DOMAIN.com` with your real URL in index.html, robots.txt and sitemap.xml
   (macOS/Linux: `sed -i 's#https://YOUR-DOMAIN.com#https://your-site.vercel.app#g' index.html robots.txt sitemap.xml`)
2. Create a GitHub repo, push this folder:
   git init && git add . && git commit -m "init" && git branch -M main
   git remote add origin https://github.com/<you>/true-size.git && git push -u origin main
3. vercel.com → Add New → Project → import the repo → Framework "Other" → Deploy. Every push to `main` now auto-deploys.
4. Google Search Console → add your URL → submit /sitemap.xml. Do the same in Bing Webmaster Tools.
