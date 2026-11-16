# Evansville Eats

A guide to where to eat in Evansville and nearby, from [@evansville_eats](https://www.instagram.com/evansville_eats/).

## Put it online with GitHub Pages (about 10 minutes, all in the browser)

1. **Sign in** at github.com (or create a free account). Your username becomes part of the web address.
2. **Make a repository.** Click **+** (top right) → **New repository**. Name it `evansville-eats`, leave it **Public**, and click **Create repository**.
3. **Upload the site.** On the new repo page, click **uploading an existing file**. Unzip the folder you got from Claude, then drag **everything inside it** (`index.html`, `README.md` and the `img` folder) into the upload box. Click **Commit changes**.
   - `index.html` must sit at the top level of the repository, not inside another folder.
4. **Turn on Pages.** Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, pick **main** and **/ (root)**, then **Save**.
5. **Wait a minute or two**, then refresh the Pages screen. Your site is live at
   `https://YOUR-USERNAME.github.io/evansville-eats/`

On the live site, visitors can type a full street address and tap **Use my location**. Both stay switched off in Claude's preview, which blocks them.

## Optional: pin every restaurant at its exact address

Distances start out using hand-placed spots. To make them exact:

1. Open your live site with `#build-geo` at the end of the address:
   `https://YOUR-USERNAME.github.io/evansville-eats/#build-geo`
2. Leave the tab open for about a minute while it looks up each address.
3. Click **Copy** when it's done.
4. In your repository, click **Add file → Create new file**, name it `geo.json`, paste, and **Commit changes**.

The site picks up `geo.json` automatically on the next visit. Anything it couldn't find keeps its estimated spot.

## Updating the site later

Edit a file on github.com (pencil icon) or upload a new `index.html` the same way as step 3. Changes go live in a minute or two.

## Optional: your own domain

Buy a domain (for example `evansvilleeats.com`), then add it under **Settings → Pages → Custom domain** and follow GitHub's DNS instructions. Check **Enforce HTTPS** once it's available, since "Use my location" only works on https.

## Credits

Address search uses OpenStreetMap's free Nominatim service (© OpenStreetMap contributors). It's meant for light use, about one search per second, which suits a site like this.
