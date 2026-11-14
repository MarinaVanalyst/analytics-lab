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

## Design

- Colours are CSS variables at the top of `styles.css` (part 1): `--indigo` #292966, `--violet` #5C5C99, `--lilac` #A3A3CC, `--periwinkle` #CCCCFF.
- `--lilac` and `--periwinkle` are too light for text on white. Use them only for lines, shapes and backgrounds.
- Font: Public Sans from Google Fonts.
- The photo is `images/marina.jpg` (400 x 400 px).

## Privacy

The contact form does not send data to a server. It does not send names, emails or messages to GA4.
