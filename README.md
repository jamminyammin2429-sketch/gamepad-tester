# Gamepad Tester

Free online controller tester for PS4 DualShock 4 and Xbox One pads, plus troubleshooting guides.

Live site: https://jamminyammin2429-sketch.github.io/gamepad-tester/

## Steps still to do (need your own accounts)

### 1. Custom domain
1. Buy a domain (Cloudflare, Porkbun or Namecheap).
2. Repo **Settings → Pages → Custom domain** → type it → Save.
3. At your registrar add DNS records:
   - `A` records for `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` for `www` → `jamminyammin2429-sketch.github.io`
4. When the check passes, tick **Enforce HTTPS**.
5. Find-and-replace `https://jamminyammin2429-sketch.github.io/gamepad-tester/` with `https://yourdomain.com/` in every `.html` file, `sitemap.xml` and `robots.txt`.

### 2. Google AdSense
1. Sign up at adsense.google.com with your new domain.
2. AdSense gives you a `<script ...adsbygoogle.js?client=ca-pub-XXXX...>` tag. In every `.html` file, paste it on the line under `<!-- ADSENSE: ... -->`.
3. Create a file named `ads.txt` in this repo containing the line AdSense shows you (it looks like `google.com, pub-XXXXXXXXXXXXXXXX, DIRECT, f08c47fec0942fa0`).
4. In AdSense, turn on **Privacy & messaging → European regulations** message (free consent banner for EU/UK visitors).
5. Request review. Turn on **Auto ads** once approved.

### 3. Amazon Associates
1. Sign up at affiliate-program.amazon.com.
2. In `parts.html`, put your tracking ID between the quotes in `const AMAZON_TAG = "";`

### 4. Google Search Console
Add your domain at search.google.com/search-console and submit `sitemap.xml` so Google finds the guides.
