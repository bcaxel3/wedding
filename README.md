# Cheyanne & Axel: wedding website

## What's in this folder

| File | What it is |
|---|---|
| `index.html` | Home page (the landing page) |
| `rsvp.html`, `registry.html`, `faq.html` | Blank pages to fill in later |
| `style.css` | All the colors, fonts and layout. The colors are at the top. |
| `images/background.jpg` | The background photo |

## Put it on GitHub Pages (no coding tools needed)

1. **Create a GitHub account** at https://github.com. Your username becomes part of the free address, like `yourusername.github.io`.
2. **Create a repository.** Click **+** (top right), then **New repository**.
   - Name: `wedding` (any name works).
   - Set it to **Public**. Free Pages hosting needs a public repository.
   - Click **Create repository**.
3. **Upload the files.** On the new repository page, click **uploading an existing file**.
   Drag in `index.html`, `rsvp.html`, `registry.html`, `faq.html`, `style.css`, and the whole **`images`** folder.
   The folder has to stay named `images`, so drag the folder itself, not just the photo inside it.
   Click **Commit changes**.
4. **Turn on Pages.** Go to **Settings**, then **Pages** (left sidebar).
   Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main**, and folder to **/ (root)**. Click **Save**.
5. **Wait about a minute and refresh.** The Pages settings will show your link:
   `https://yourusername.github.io/wedding/`

### Making changes later
Open any file on GitHub, click the **pencil icon**, edit, then click **Commit changes**. The site updates within about a minute.
(Hard-refresh your browser with Ctrl+Shift+R if you still see the old version.)

## Adding your own domain later

1. Buy the domain (from Cloudflare, Porkbun or Namecheap, for example).
2. On GitHub, go to **Settings**, then **Pages**, then **Custom domain**. Type in `yourdomain.com` and click **Save**.
3. In your domain company's DNS settings, add these records:
   - Four **A** records for `@`, pointing to
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - One **CNAME** record for `www`, pointing to `yourusername.github.io`
4. After it connects (anywhere from minutes to a few hours), tick **Enforce HTTPS** on the same settings page.

Every link inside the site is relative, so the site works the same on the github.io address and on your own domain.
