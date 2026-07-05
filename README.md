# 11+ Exam Prep — Daily Practice

Static site for Sutton Grammar 11+ daily Maths & English practice sessions.

## Structure

```
index.html          ← Dashboard — links to all days
days/
  day-01.html       ← Day 1 session
  day-02.html       ← Day 2 session (add as you go)
  ...
_config.yml         ← GitHub Pages config
```

## Adding a new day

1. Copy `days/day-01.html` to `days/day-XX.html` (zero-padded, e.g. `day-02.html`)
2. Update the questions and answers inside the file
3. In `index.html`, find the matching day entry in the `days` array and set `available: true` and update the `title`
4. Commit and push — GitHub Pages deploys automatically

## Enabling GitHub Pages

In your repo → **Settings → Pages → Source**: deploy from the branch you push to, root folder `/`.
