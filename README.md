# Gabriel's Portfolio – Setup & Publishing Guide

## Files
| File | Purpose |
|---|---|
| `index.html` | The whole website (HTML + CSS + JavaScript in one file) |
| `photo.jpg` | **You add this.** Your formal portrait |

Until `photo.jpg` exists, the homepage shows a green "GP" placeholder.

## 1. Add your photo
- Use a real formal photo: plain light or dark background, collared shirt or blazer, facing the camera, good lighting.
- Crop it to **4:5 portrait** (for example 800 × 1000 px).
- Save it as `photo.jpg` in the same folder as `index.html`.
- If your instructor allows an AI-generated portrait, it still needs to look natural. A real photo of you is the safer choice.

## 2. Edit the content
Open `index.html` in any text editor (VS Code is good). Search for text and replace it. Colors are at the top, in the `:root { ... }` block:
`--green` is the accent, `--bg` is the black background, `--white` is the heading color.

To test, double-click `index.html`. Use the Previous/Next buttons or the left/right arrow keys.

## 3. Publish on GitHub Pages
1. Create a free account at github.com.
2. Click **New repository**. Name it anything (for example `portfolio`). Set it to **Public**.
3. Click **uploading an existing file** and upload `index.html` and `photo.jpg`. Click **Commit changes**.
4. Go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
5. After a minute or two your site is live at `https://YOUR-USERNAME.github.io/portfolio/`.

## 4. The "www." requirement (important)
A free GitHub address (`username.github.io`) does **not** start with `www.`, so on its own it does not meet the requirement. To get a URL that starts with `www.`, you need a **custom domain**:

1. **Buy a domain** from a registrar (Namecheap, Porkbun, GoDaddy, etc.). Prices vary, and typically a `.com` costs around US$10–15 per year. Check whether any student offer you qualify for includes a free domain. Choose a name like `gabrielpingay.com`.
2. **Add the domain in GitHub:** repository **Settings → Pages → Custom domain**, type `www.gabrielpingay.com` (your own domain), and **Save**. GitHub creates a file called `CNAME` in your repository automatically. Do not create it with a fake domain.
3. **Set DNS records** at your registrar's DNS page:
   - **CNAME**: Host `www` → Value `YOUR-USERNAME.github.io`
   - Optional, so the bare domain also works: four **A** records for host `@` pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
4. Wait for DNS to update (a few minutes to 24 hours). In **Settings → Pages**, once the DNS check passes, tick **Enforce HTTPS**.
5. Visit `https://www.gabrielpingay.com`. Submit that exact `www.` link.

Check GitHub's current instructions at docs.github.com ("Managing a custom domain for your GitHub Pages site") in case anything has changed.

## 5. Requirement checklist
- [x] Separate pages: Home, About, Education, Achievements, Skills, Career Goals, Contact
- [x] No scrolling: each page is one fixed screen
- [x] Previous / Next buttons in the same bottom bar on every page
- [x] Buttons that reveal extra details (quick facts, what I'm learning, what's next, skills tabs, copy email)
- [x] Black, green and white design
- [ ] Formal photo: add `photo.jpg`
- [ ] URL starting with `www.`: set up your custom domain (step 4)

## Troubleshooting
- **Photo not showing:** the file must be named exactly `photo.jpg`, lowercase, in the same folder as `index.html`.
- **Page needs scrolling on your screen:** very small windows may need a little scrolling inside a page. Zoom the browser out slightly (Ctrl and minus) or shorten your text.
- **Changes not appearing online:** wait a minute, then hard refresh (Ctrl + Shift + R).
