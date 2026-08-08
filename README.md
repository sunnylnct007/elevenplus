# 11+ Exam Prep — Daily Practice

Static site for Sutton Grammar 11+ daily Maths, English, Verbal Reasoning & Non-Verbal Reasoning practice sessions.

## Structure

```
index.html          ← Dashboard — links to all days
days/
  day-01.html       ← Day 1 session
  day-02.html       ← Day 2 session
  day-03.html       ← Day 3 session
  ...
samples/            ← Reference 11+ practice papers (not part of the site)
_config.yml         ← GitHub Pages config
```

## Samples

The `samples/` folder holds the original 11+ practice papers (Maths, English, Verbal
Reasoning, Non-Verbal Reasoning) used as a style reference. Days 2 and 3 were written
from scratch in the same multiple-choice (A–E) exam format, extended to also cover
Verbal and Non-Verbal Reasoning alongside Maths and English.

## Adding a new day

1. Copy `days/day-02.html` to `days/day-XX.html` (zero-padded, e.g. `day-04.html`) — it has the full Maths/English/VR/NVR template
2. Update the questions and answers inside the file, and fix the prev/next links in `.nav-row`
3. In `index.html`, find the matching day entry in the `days` array and set `available: true` and update the `title`
4. Commit and push — GitHub Pages deploys automatically

## Enabling GitHub Pages

In your repo → **Settings → Pages → Source**: deploy from the branch you push to, root folder `/`.
