OSCAR BOWEN-HILL SITE: HOW TO PUBLISH ON GITHUB PAGES

Files: index.html (the page), images/ (photos), fonts/ (add the 3 font files, see fonts/README.txt), CNAME (your domain), .nojekyll (leave as is).

1. Create a free GitHub account, then a NEW PUBLIC repository (free Pages needs a public repo). Name it e.g. oscartenor.
2. Unzip this package. In the repository choose Add file > Upload files and drag in EVERYTHING inside the unzipped folder (index.html, CNAME, .nojekyll and the images and fonts folders). Commit.
3. Repository Settings > Pages > Source: Deploy from a branch, branch main, folder /(root). Save.
4. Same page, Custom domain: type oscartenor.com and Save. Do this BEFORE changing DNS.
5. At the company where you bought oscartenor.com, open DNS settings and add:
   A records for @ : 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   CNAME record for www : YOUR-GITHUB-USERNAME.github.io
   (Optional IPv6 AAAA records for @ : 2606:50c0:8000::153, 2606:50c0:8001::153, 2606:50c0:8002::153, 2606:50c0:8003::153)
   Remove any old A or CNAME records for @ and www that point elsewhere.
6. Wait (up to 24 hours). When Pages shows the DNS check passed, tick Enforce HTTPS.
7. Recommended: GitHub profile Settings > Pages > Add a domain, to verify oscartenor.com and prevent takeovers.

TO EDIT LATER: in the repository open index.html, click the pencil icon, change text, commit. Replace a photo by uploading a new file with the same name into images/.
VIDEOS: in index.html find data-yt="" and put the YouTube video ID between the quotes (the 11 characters after /shorts/ or v=).
BEFORE LAUNCH: in impressum.html and datenschutz.html replace every orange [bracketed placeholder] (your own postal address; delete the VAT-ID line if you have none). Use your own address, not your employer's. Have both pages checked by a lawyer or an Impressum/privacy service.

WATCH SECTION: the Britten and Bach video tiles were removed for launch. Add them back later by asking Claude, or copy a tile and set data-yt to the YouTube ID.
