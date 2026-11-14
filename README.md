# Marina V. Analytics Lab

A practice website for Google Tag Manager and GA4. It is hosted free on GitHub Pages.

Live site: https://marinavanalyst.github.io/

## Pages

| Page | page_type | What to track |
| --- | --- | --- |
| index.html | home | CTA button clicks (ids `cta-projects`, `cta-contact`) |
| about.html | info | Spreadsheet download |
| projects.html | projects | Outbound links (class `project-link`), spreadsheet download |
| guide.html | article | Scroll depth, spreadsheet and PDF downloads (video optional) |
| contact.html | lead | `generate_lead` event from the form |

Downloads:

- `files/tracking-plan.pdf`: the tracking plan for this site.
- `files/multi-site-tracking-plan.xlsx`: my framework to plan, check and report tracking across many websites.

## Before you publish

1. Each page has `<meta name="robots" content="noindex, nofollow">`. It stops search engines from showing the draft. Remove it from each page when the site is finished.
2. Install Google Tag Manager: paste the 2 GTM codes where each page says LESSON 1.
3. Optional: to practise video tracking, add a YouTube video in `guide.html`. The steps are in a comment in the file.

## Design

- Colours are CSS variables at the top of `styles.css` (part 1): `--indigo` #292966, `--violet` #5C5C99, `--lilac` #A3A3CC, `--periwinkle` #CCCCFF.
- `--lilac` and `--periwinkle` are too light for text on white. Use them only for lines, shapes and backgrounds.
- Font: Public Sans from Google Fonts.
- The photo is `images/marina.jpg` (400 x 400 px).

## Privacy

The contact form does not send data to a server. It does not send names, emails or messages to GA4.
