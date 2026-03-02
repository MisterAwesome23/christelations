# Deploying Christelation to GitHub Pages

This guide walks Rick (or Akshat) through deploying the Christelation website — step by step, no experience needed.

---

## Before You Start

You'll need:
- A **GitHub account** (free) — sign up at [github.com](https://github.com) if you don't have one
- **Git** installed on your computer — download from [git-scm.com](https://git-scm.com)
- The entire **Christelation folder** (the one containing `index.html`)

---

## Step 1 — Add Your Phone Number

Before deploying, open `index.html` in any text editor (TextEdit, Notepad, VS Code).

Search for `(XXX) XXX-XXXX` — it appears **3 times**. Replace all three with Rick's real phone number.

Also find `tel:+1XXXXXXXXXX` (appears 3 times) and replace with the actual number in format `tel:+17815551234`.

Save the file.

---

## Step 2 — Create a GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the **+** button (top right) → **New repository**
3. Name it: `christelation` (all lowercase)
4. Set it to **Public**
5. Do **NOT** check "Add a README file"
6. Click **Create repository**

---

## Step 3 — Upload the Files

In your terminal (Mac: Terminal app / Windows: Git Bash or Command Prompt), run:

```bash
# Navigate to the Christelation folder
cd /path/to/your/Christelation

# Initialize git and push everything
git init
git add .
git commit -m "Launch Christelation website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/christelation.git
git push -u origin main
```

> Replace `YOUR-USERNAME` with your actual GitHub username.

**Alternative — Drag & Drop:**
If you prefer not to use Terminal, on your new GitHub repository page, click **"uploading an existing file"** and drag the entire Christelation folder contents in.

---

## Step 4 — Enable GitHub Pages

1. On your GitHub repository page, click **Settings** (top tab)
2. In the left sidebar, click **Pages**
3. Under **Source**, select **Deploy from a branch**
4. Under **Branch**, choose `main` and folder `/root`
5. Click **Save**

GitHub will show you a message like:
> "Your site is live at https://YOUR-USERNAME.github.io/christelation/"

It usually takes **1–3 minutes** to go live.

---

## Step 5 — Visit Your Live Site

Go to:
```
https://YOUR-USERNAME.github.io/christelation/
```

That's it — the website is live!

---

## Optional: Custom Domain (e.g. christelation.com)

If Rick wants a real domain name like `christelation.com`:

1. Purchase the domain from [Namecheap](https://namecheap.com) or [Google Domains](https://domains.google)
2. In GitHub Pages settings, enter the domain under **Custom domain**
3. Follow GitHub's DNS setup instructions (they walk you through it)

Cost: ~$12/year for a `.com` domain. Hosting on GitHub Pages is **free**.

---

## Updating the Site Later

To make changes (e.g. update phone number, add photos):

1. Edit the files locally
2. Run:
```bash
git add .
git commit -m "Update site"
git push
```
The site updates automatically within a few minutes.

---

## Questions?

Contact Akshat (LegitReach Analyst) or reach out through LegitReach for support.
