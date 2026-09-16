# Contributing a case

Plan on two to four hours for a first case. The write-up matters more than the code.

## Steps

1. **Fork** this repository (button top right), then clone your fork.
2. **Create a folder** for your case: `cases/<major>/<yyyy-mm>-<short-slug>/`
   Example: `cases/cybersecurity/2026-10-phishing-detection-sigma/`
3. **Copy the template** from `cases/_template/README.md` into your folder and fill in every section.
   Put notebooks, scripts, images and small data files (under 5 MB) in the same folder.
4. **Commit and push** to your fork, then open a **pull request** against `main`. The pull request
   template asks you three questions; answer them in a sentence each.
5. An automatic Semgrep security scan runs on your pull request (secrets, injection, unsafe code). If it
   fails, open the "Checks" tab, fix what it points at, and push again. It never blocks a write-up-only case.
6. A TLDP staff member reviews within a week. Address comments by pushing more commits to the same
   branch. When it merges, the bot posts your case in Discord.

## What makes a case good

- **A real question.** "Which NYC neighborhoods lost the most bus ridership after the 2025 fare
  change?" beats "an analysis of bus data".
- **Real data or a real scenario**, cited with a link. Public sources only.
- **Honest results.** Say what didn't work. A case with a negative result is still a case.
- **Reproducible.** Someone should be able to rerun your notebook from the files in the folder.
- **Short.** 600–1500 words in the README. Details go in the notebook.

## Checklist before you open the pull request

- [ ] Folder name follows `cases/<major>/<yyyy-mm>-<slug>/`
- [ ] Every template section is filled in (delete the hints)
- [ ] Data source is linked and public; no personal data, credentials, or NDA material
- [ ] Any code runs from the folder as-is
- [ ] Images are under 1 MB each; data files under 5 MB (link larger data instead)
- [ ] Your name in the README is how you want it to appear publicly

## Working from an existing collection

If your case is a contribution to an outside collection (Tidy Tuesday, Atomic Red Team, Sigma,
OWASP, Open Case Studies, Makeover Monday…), still write it up here: link the upstream pull request
or publication in the "Result" section. That's the version recruiters will read.

## Code of conduct

Be the colleague you'd want to work with. Reviews are about the work, never the person.
