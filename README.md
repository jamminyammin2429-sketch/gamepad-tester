# Ultimate Controller

Free online controller tester for PS4 DualShock 4 and Xbox One pads, plus troubleshooting guides.

Live site: https://ultimatecontroller.com/

## Steps still to do (need your own accounts)

### 1. Custom domain — done
ultimatecontroller.com (Cloudflare Registrar, DNS only) → GitHub Pages. Keep the `CNAME` file in this repo.

### 2. Google AdSense
1. Sign up at adsense.google.com with your new domain.
2. Done: the AdSense script (ca-pub-1083294266156352) is in every page and `ads.txt` is in the repo.
4. In AdSense, turn on **Privacy & messaging → European regulations** message (free consent banner for EU/UK visitors).
5. Request review. Turn on **Auto ads** once approved.

### 3. Amazon Associates
1. Sign up at affiliate-program.amazon.com.
2. In `parts.html`, put your tracking ID between the quotes in `const AMAZON_TAG = "";`

### 4. Google Search Console
Add your domain at search.google.com/search-console and submit `sitemap.xml` so Google finds the guides.
