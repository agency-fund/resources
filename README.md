# The Agency Fund — Resources

This repo is the website at **https://agency-fund.github.io/resources/**. Every resource lives in its own folder, and the folder name becomes its web address:

| Folder | Live at |
| --- | --- |
| `graduation/` | https://agency-fund.github.io/resources/graduation/ |
| `noora-neurips-case-study/` | https://agency-fund.github.io/resources/noora-neurips-case-study/ |
| `psych-poverty-reduction/` | https://agency-fund.github.io/resources/psych-poverty-reduction/ |

There is no build step. You can do everything below in the GitHub website.

## Add a new resource

**1. Pick a short folder name** (the "slug"): lowercase, words joined by hyphens, e.g. `cash-transfers-review`.

**2. Add the files.** On the repo's main page, click **Add file → Upload files**.

- **If you have a web page** (an `.html` file): rename it to `index.html` on your computer first. Then, on the upload screen, drag in a folder named after your slug that contains `index.html`. (You can also use **Add file → Create new file** and type `your-slug/index.html` as the name; the `/` creates the folder.)
- **If you have a PDF**: drag in a folder named after your slug that contains the PDF. Give the PDF a descriptive name with no spaces, e.g. `smith-2026-cash-transfers-review.pdf`. If you want a landing page too, copy `noora-neurips-case-study/index.html` into your folder and edit the text.

Scroll down, write a short message like "Add cash transfers review", choose **Commit directly to the main branch**, and click **Commit changes**.

**3. List it on the home page.** Open `index.html` (in the top level of the repo) and click the pencil icon to edit. Copy one whole card, from `<li class="card">` down to its matching `</li>`, and paste it into the list. Change the tag, title, authors, venue/date, one-line blurb, and both links to point at your folder, e.g. `href="cash-transfers-review/"`.

Links must **not** start with `/`. Write `cash-transfers-review/`, not `/cash-transfers-review/`, or the link will break.

Commit the change to `main` the same way.

## When does it go live?

A minute or two after the change is committed to `main`, it appears at `https://agency-fund.github.io/resources/<slug>/`. If it doesn't show up, wait another minute and refresh. The **Actions** tab shows whether the publish finished.

## Styling

Shared colors and fonts (from the graduation report) are in `assets/site.css`. Pages can use it with `<link rel="stylesheet" href="../assets/site.css">`.
