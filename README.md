# ArelSystem

A personal RPG: daily fitness and discipline quests, XP, six stats, levels, Hunter ranks, streaks, achivements.
## Run it
Just open `index.html` in a browser — no build step, no server. All progress is saved to that browser's local storage, on that device.

To use it from your phone and laptop with the same look (not the same save data), you can also enable **GitHub Pages**: Settings → Pages → Deploy from branch → `main` → `/ (root)`. You'll get a public URL that opens the app from anywhere.

## First run
On first open, the System asks for your fitness level, available equipment, and primary goal, then generates your starting stats and today's quests. Quest difficulty (push-up/squat/sit-up counts, distance, step target) scales automatically with your level.

## Commands (as buttons)
`/daily` current quests · `/quest` a special one-off challenge · `inventory` achievements · `/rank` Hunter rank · `/report` last 7 days · `/rest` a recovery-day plan that protects your streak · `/status` full profile · level up progress.

## Setup on GitHub
```
git init
git add .
git commit -m "Initial System build"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

## Releases
Push a version tag any time you want a packaged release artifact:
```
git tag v1.0.0
git push origin v1.0.0
```
The included workflow (`.github/workflows/release.yml`) zips the app and attaches it to a GitHub Release automatically. You can also trigger it manually from the Actions tab (`workflow_dispatch`) without tagging — it'll upload the zip as a workflow artifact.

## Notes
- No external accounts, servers, or data collection — everything runs and stays in your browser.
- "Reset System" on the Status tab wipes local progress on that device if you ever want to restart from Level 1.
- 
