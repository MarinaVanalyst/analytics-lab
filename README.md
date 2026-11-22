# Marina V. Analytics Lab

> **Work in progress.** I am a beginner in web analytics, and I am still learning. I build this site step by step, and some parts are not tracked yet.

A practice website for Google Tag Manager and GA4. It is hosted free on GitHub Pages.

Live site: https://marinavanalyst.github.io/analytics-lab/

## Where I am in my learning

| Step | Status |
| --- | --- |
| Install Google Tag Manager on all pages | Done |
| Connect GA4, and test page views in DebugView | Done |
| Set automatic events, so that nothing counts twice | Done |
| Read page data with dataLayer variables | Next |
| Track button clicks, downloads and the contact form | Not started yet |
| Add a cookie consent banner | Not started yet |
| Check data quality on a schedule | Not started yet |
| Build my first report in Looker Studio | Not started yet |

## Tracking setup

- Google Tag Manager container: `GTM-W2N66H9H` (in the head of all 5 pages, after the dataLayer code)
- GA4 Measurement ID: `G-5K823425JY` (in GTM, Google Analytics tag on Initialization - All Pages)
- Automatic events: only page views, in GA4 and in the GTM container settings

## Pages

| Page | page_type | What to track |
| --- | --- | --- |
| All pages | | Menu button (id `nav-contact`), footer links to LinkedIn and GitHub |
| index.html | home | Buttons (ids `cta-projects`, `cta-contact`, `cta-guide`), questions that open and close |
| about.html | info | Spreadsheet download |
| projects.html | projects | Outbound links (class `project-link`), spreadsheet download |
| guide.html | article | Scroll depth, spreadsheet and PDF downloads |
| contact.html | lead | `generate_lead` event from the form |

Downloads:

- `files/tracking-plan.pdf`: the tracking plan for this site.
- `files/multi-site-tracking-plan.xlsx`: my framework to plan, check and report tracking across many websites.

## Before the site is finished

1. Each page has `<meta name="robots" content="noindex, nofollow">`. It stops search engines from showing the draft. Remove it from each page when the site is finished.
2. Optional: to practise video tracking, add a YouTube video in `guide.html`. The steps are in a comment in the file.

## Design

- Dark theme, inspired by modern portfolio builder websites: floating pill menu, centred headings, dark rounded cards, questions that open and close.
- Colours are CSS variables at the top of `styles.css` (part 1). Palette: `--indigo` #292966, `--violet` #5C5C99, `--lilac` #A3A3CC, `--periwinkle` #CCCCFF.
- Font: Manrope from Google Fonts.
- The photo is `images/marina.jpg` (400 x 400 px).

## Privacy

The contact form does not send data to a server. It does not send names, emails or messages to GA4.
