# EXAMPLE — Which week of Tidy Tuesday drew the most community submissions in 2026?

**Author:** TLDP Staff (example case) · **Major:** Data Analytics · **Date:** 2026-09 · **Level:** starter

> This is a worked example of the shape we expect. Replace it with your own case. Numbers below are
> illustrative placeholders, not real findings.

## The situation

Tidy Tuesday publishes a new public dataset every week. Students choosing which week to analyze
want to know which datasets attract the most community work, because those weeks have the most
examples to learn from.

## The question

Which 2026 Tidy Tuesday weeks have the most public submissions, and what do those datasets have in common?

## Data or scenario

- Source: https://github.com/rfordatascience/tidytuesday (the `data/2026` folder and each week's readme)
- Size and shape: one folder per week, each with a CSV and a readme describing the source
- Known limits: submission counts are self-reported on social media, so this is a proxy, not a census

## What I did

1. Listed the 2026 week folders with the GitHub contents API (Python, `urllib`).
2. Read each readme and recorded the dataset topic and row count.
3. Counted public submissions per week from the community hashtag archive.
4. Plotted submissions against dataset size and topic (`analysis.ipynb`, `submissions.png`).

## Result

Weeks with small, tidy datasets on everyday topics (sports, food, transit) drew the most submissions.
Dataset size had little effect; topic familiarity had a lot. See `submissions.png`.

## What I'd do next

- Check whether the pattern holds for 2025
- Add a "time to first submission" measure
- Compare Python versus R submissions per week

## What I learned

Pick a dataset you already have questions about; the analysis goes faster and the write-up is
better. Scraping the hashtag archive was the slowest step and the least reliable. Next time I'd
sample two weeks by hand first.
