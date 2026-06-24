# How to Set Up Your GitHub Profile README

Your profile README is what visitors see at [github.com/Deep95y](https://github.com/Deep95y). Follow these steps to go live.

## Step 1: Create the Special Repository

GitHub only shows a profile README from a repo named **exactly** like your username.

1. Go to [github.com/new](https://github.com/new)
2. Set **Repository name** to: `Deep95y` (must match your username exactly)
3. Set visibility to **Public**
4. Check **Add a README file** (optional — you'll replace it)
5. Click **Create repository**

## Step 2: Upload These Files

### Option A — GitHub Web UI (easiest)

1. Open your new `Deep95y/Deep95y` repo
2. Delete the default `README.md` if one exists
3. Click **Add file → Upload files**
4. Upload `README.md` from this folder
5. Upload `.github/workflows/snake.yml` (create folders as needed)
6. Commit the changes

### Option B — Git CLI

```bash
cd C:\Users\VJ\github-profile-deep95y

git init
git add README.md .github/workflows/snake.yml
git commit -m "Add GitHub profile README"
git branch -M main
git remote add origin https://github.com/Deep95y/Deep95y.git
git push -u origin main
```

## Step 3: Enable the Contribution Snake

1. In your `Deep95y` repo, go to **Actions**
2. Click **"I understand my workflows, go ahead and enable them"**
3. Select **Generate Snake** → **Run workflow**
4. After it runs (~1 min), the snake SVG appears at `output/github-contribution-grid-snake.svg`

The snake auto-updates daily via the scheduled workflow.

## Step 4: Pin Your Best Repositories

1. Go to [github.com/Deep95y](https://github.com/Deep95y)
2. Click **Customize your pins**
3. Select up to 6 repos, for example:
   - Event-Management
   - notes-management
   - Dream-Music
   - Automation-system
   - ContentOnContext
   - devops-microservices-platform

## Step 5: Customize Your Profile (Optional)

On [github.com/settings/profile](https://github.com/settings/profile):

| Field | Suggested value |
|-------|-----------------|
| **Name** | Deepa Yadav |
| **Bio** | Full Stack Web Developer \| MERN \| Mumbai |
| **Location** | Mumbai, India |
| **Website** | https://depportfolio.netlify.app/ |
| **Twitter** | @DeepaYadav79409 |

## Step 6: Personalize the README

Edit `README.md` to update:

- **LinkedIn URL** — replace the placeholder if your handle differs
- **Projects** — add or remove rows in the Featured Projects table
- **Tech stack** — add/remove badge lines
- **Typing animation lines** — change the `lines=` parameter in the Typing SVG URL
- **Theme** — swap `tokyonight` for `dracula`, `radical`, `merko`, etc. in stats URLs

## Troubleshooting

| Issue | Fix |
|-------|-----|
| README not showing on profile | Repo must be **public** and named **Deep95y** exactly |
| Stats cards show 404 | Make some repos public; stats need public activity |
| Snake image broken | Run the **Generate Snake** workflow once in Actions |
| Badges not loading | External services can be slow; refresh after a few minutes |

## File Structure

```
Deep95y/                    ← repo name = your username
├── README.md               ← your profile page content
└── .github/
    └── workflows/
        └── snake.yml       ← auto-generates contribution snake
```

Once pushed, visit [github.com/Deep95y](https://github.com/Deep95y) to see your new profile.
