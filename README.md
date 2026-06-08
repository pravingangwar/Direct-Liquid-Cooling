# Rack-Level Direct Liquid Cooling — Thermal System Design Review

A single-page, self-contained portfolio website presenting a full thermal-hydraulic design review of a 90 kW direct-liquid-cooled compute rack.

Author: **Pravin Kumar** · pravink7@outlook.com

## Files
- `index.html` — the entire website (HTML, CSS, JS, and the loop schematic are all inline; the only external dependency is Google Fonts loaded over CDN). No build step.

## Deploy to GitHub Pages

### Option A — repo named for a project page
1. Create a new GitHub repository, e.g. `Direct-Liquid-Cooling`.
2. Add `index.html` to the repository root and commit:
   ```bash
   git init
   git add index.html README.md
   git commit -m "Rack-level DLC design review site"
   git branch -M main
   git remote add origin https://github.com/pravingangwar/Direct-Liquid-Cooling.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, select **Deploy from a branch**.
5. Choose branch **main** and folder **/ (root)**, then **Save**.
6. After a minute the site is live at:
   `https://pravingangwar.github.io/Direct-Liquid-Cooling/`

### Option B — user/organization site (root domain)
Name the repository exactly `<your-username>.github.io`, push `index.html` to the root, enable Pages as above, and the site serves at `https://pravingangwar.github.io/`.

## Custom domain (optional)
Add a file named `CNAME` containing your domain (e.g. `dlc.pravinkumar.dev`), commit it, then set the matching DNS records and enter the domain under **Settings → Pages → Custom domain**.

## Editing
Open `index.html` in any editor. Content lives in clearly labeled `<section>` blocks (`#budget`, `#arch`, `#resistance`, `#cdu`, `#hydraulics`, `#balancing`, `#pump`, `#coldplate`, `#controls`, `#materials`, `#summary`). Colors are CSS variables in the `:root` block near the top.
