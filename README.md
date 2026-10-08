# Farhan Hossain - Personal Portfolio

INFR3120U Assignment 1: a personal portfolio using HTML5 and CSS3.

## Website and repository

Live website:
https://fhossain-dev.github.io/infr3120-portfolio/

Public repository:
https://github.com/fhossain-dev/infr3120-portfolio

## Current progress

- Created four separate HTML pages with shared navigation and footers.
- Added the colour palette, gradients, and responsive stylesheets.
- Added the About-page portrait and HTML5 introduction video.
- Added four project entries with shared card styling.
- Published the portfolio using GitHub Pages.
- All four HTML pages and all four CSS stylesheets passed validation.
- Completed link checking, spelling checking, WAVE checks, and manual keyboard testing.
- Further media accessibility review remains pending, including synchronized captions.
- Added and locally tested the responsive Contact form.

## Projects page
Four project entries use separate HTML5 article elements,
each with a heading and a short description.

The card appearance was adapted from the supplied course
stylesheet, style(1)(1).css. Smartphone styling reduces card
padding to fit narrower screens.

AI helped draft the descriptions from my project information
and guided the HTML integration and responsive styling.

## Contact form

The form includes Name, Email, Cell number, Comments, and Submit.
All four fields are required. HTML5 email validation checks the
email format, and the phone pattern requires exactly 10 digits.

The form uses the mailto approach from the Week 2
course notes. It opens the visitor's configured email application
with the recipient and entered information. The visitor must
review and send the email because the website does not send it
automatically.

The form structure, labels, textarea, submit control, and required
and email validation were adapted from the Week 2 course examples.
The telephone input and pattern validation were added with some AI
guidance and reference to the WHATWG HTML Standard:
https://html.spec.whatwg.org/dev/input.html

AI also helped assemble the form CSS when stuck or confused, explain
validation, as well as support with course material, also helped
identify quotation-mark errors in the opening form tag.

### Local form testing — October 7, 2026

Tested in Opera browser on Windows:
- Blank Name, Email, Phone, and Comments were each blocked.
- Email 'hello' was rejected.
- Phone '12345' and 'abcdefghij' were rejected.
- Valid details opened an Outlook draft containing a recipient
  and all four entered values.

### Deployed website testing — October 7, 2026

All four pages opened on GitHub Pages. The About-page portrait loaded
and the introduction video played.

Valid Contact form details opened an Outlook draft with the correct
recipient and all four entered values. The draft was closed without
sending an email.

Opera browser displayed a security warning during the mailto submission.
Continuing past the warning opened the populated email draft.
The form depends on the visitor's configured email application.

## Assistance

AI assisted with Git and VS Code setup, explaining
HTML and CSS based on supplied course examples, drafting project
descriptions from my information, debugging, and interpreting tests.

Course sources and the additional telephone-validation reference
are identified in the relevant sections of this README.

## Colour scheme

The palette was created using the Analogous harmony in Adobe Color:
https://color.adobe.com/create/color-wheel

| Colour | Hex code | Use |
| --- | --- | --- |
| Dark blue | #0B3C5D | Header background and gradient |
| Teal | #0B555C | Header gradient |
| Navy | #0B225C | Body text and footer gradient |
| Dark green | #0B5C48 | Navigation hover and focus |
| Indigo | #0E0B5C | Footer gradient |

White (#FFFFFF) and pale grey (#F4F9F9) provide neutral
backgrounds for the content.

The blue and teal colours suit the technology focus of my
portfolio. Dark text on white content areas makes the text
easy to read, while green highlights navigation interactions. 

## Gradients

Both gradients are defined in css/base.css and appear on
all four pages.

- Header: linear-gradient(to right, #0B3C5D, #0B555C).
  This is a horizontal linear gradient from dark blue to teal.
- Footer: linear-gradient(135deg, #0B225C, #0E0B5C).
  This is an angled linear gradient from navy to indigo.

## Navigation layout

The navigation uses floated list items and a clearing element.
Links appear four across on larger screens, two across on tablet
screens, and vertically on phone screens. Hover and keyboard focus
highlight the links. No Flexbox is used.

## Responsive layout

All four pages include the viewport meta tag and share these stylesheets:

- css/base.css: shared colours, typography, and page styling.
- css/full.css: default layout with an 80% main content width.
- css/tablet.css: applies at widths of 960px or below.
  Main content uses 90% width and navigation links use 50% width.
- css/smartphone.css: applies at widths of 480px or below.
  Main content uses 95% width and navigation links stack vertically.

The 480px and 960px breakpoints follow the examples taught in the course lectures.
Percentage widths let the content adjust between breakpoints.
Smaller screens use more of the available width and reduced padding.

The default stylesheet loads first, followed by tablet and phone
overrides. On phones, both smaller screen stylesheets apply, with
the phone rules taking priority because they load last.

## Testing so far

Initial desktop and tablet visual checks were completed.
Initial responsive checks at 375 x 800 showed that navigation,
text, and footers fit. A final responsive and browser Console check
of the deployed pages after the media and form changes is pending.

Formal HTML and CSS validation passed on October 7, 2026.
Link, spelling, WAVE, and manual keyboard checks were completed
on October 8, 2026. Further media accessibility review remains
pending, including synchronized captions.

- Checked the Projects page at 375 × 800: all four cards,
  navigation, and footer fit without visible horizontal overflow.
  No page errors appeared in the browser Console.

## About-page media

- Portrait: images/farhan.jpeg, with descriptive alternative text.
- Introduction recording: videos/introduction.mp4.
- The portrait is also used as the video's poster image.
- The HTML5 player includes native controls and fallback content.
- The portrait and video scale down to fit smaller screens.

The portrait and recording feature Farhan Hossain.
The video markup was adapted from the INFR3120U Week2 course notes,
pages 4–7, with some AI guidance for integration into this portfolio.
AI also helped assemble and explain the responsive media styling.

The video player was visually checked on desktop and at 375px width.

## HTML and CSS validation

Tested the published GitHub Pages files on October 7, 2026.

### HTML — W3C Nu HTML Checker
https://validator.w3.org/nu/

| Page | Errors | Warnings |
| --- | --- | --- |
| index.html | 0 | 0 |
| about.html | 0 | 0 |
| projects.html | 0 | 0 |
| contact.html | 0 | 0 |

About and Contact were revalidated on October 8, 2026,
after adding the video transcript and explicitly closing
the first Contact paragraph. Both returned no errors or warnings.

### CSS — W3C CSS Validation Service
https://jigsaw.w3.org/css-validator/

Profile: CSS level 3 + SVG.

| Stylesheet | Result |
| --- | --- |
| css/base.css | No errors found; no warnings reported |
| css/full.css | No errors found; no warnings reported |
| css/tablet.css | No errors found; no warnings reported |
| css/smartphone.css | No errors found; no warnings reported |

## Project files

| File or folder | Purpose |
| --- | --- |
| index.html | Home page |
| about.html | Introduction, portrait, and video |
| projects.html | Four project descriptions |
| contact.html | Contact form |
| css/base.css | Shared styling |
| css/full.css | Default desktop layout |
| css/tablet.css | Tablet layout overrides |
| css/smartphone.css | Phone layout overrides |
| images/farhan.jpeg | Portrait and video poster |
| videos/introduction.mp4 | Introduction video |
| README.md | Documentation, credits, and test results |

## Running locally

Download and extract the repository ZIP, or clone the repository.
Keep the files and folders together, then open index.html in a browser.
Use the navigation links to visit the other three pages.
No installation or build step is required.

The Contact form requires a configured email application.
Submitting prepares a draft where the visitor must send it themselves.

## GitHub Pages deployment

The public repository publishes from the main branch and root folder.

In GitHub Settings > Pages, the source is "Deploy from a branch",
with main and /(root) selected.

Changes are saved locally, staged and committed using the terminal,
then uploaded with git push. The updated website is checked after
the Pages deployment finishes successfully in GitHub Actions.

## Author

Farhan Hossain.
Course adaptations, external references, and AI assistance are
described in the relevant sections above.

## Link checking — October 8, 2026

Tested the published website using the W3C Link Checker:
https://validator.w3.org/checklink

Recursive checking was enabled with a depth of 1.
The checker processed 9 documents, covering all four HTML
pages and the shared stylesheets. The About-page portrait
and introduction video URLs were also checked.

No broken HTTP or HTTPS links were reported.
The checker reported N/A notices for the footer email links
because checking mailto URLs is disabled in the service.

Contact form submission was tested separately and opened
an Outlook draft, as documented above.

## WAVE accessibility checking — October 8, 2026

Checked all four published pages using https://wave.webaim.org/.

| Page | Errors | Contrast errors | Alerts |
| --- | --- | --- | --- |
| Home | 0 | 0 | 0 |
| About | 0 | 0 | 2 |
| Projects | 0 | 0 | 0 |
| Contact | 0 | 0 | 0 |

WAVE recognized all four Contact form labels.

The About-page alerts were "Audio/Video" and
"HTML5 video or audio", relating to the MP4 link and video player.
These require manual review of media accessibility, including
captions, a transcript, and keyboard controls.

These automated results do not establish full accessibility.
Manual keyboard checks were completed as documented below.
Further media accessibility review remains pending.

### Manual keyboard testing — October 8, 2026

Tested on the published website in Opera browser on Windows:
- Navigation links showed visible keyboard focus and opened with Enter
  across all four pages.
- The About-page video could be played and paused using the keyboard,
  and focus could move away from the player.
- Contact fields and Submit were reachable in the expected order.
  Focus was visible, and all four fields accepted typed input.

A transcript is available beneath the About-page video.
Synchronized captions are still pending.

## Spelling check — October 8, 2026

The published text from all four pages, including the About-page
video transcript, was checked using Microsoft Word Editor with
English (Canada) selected. No spelling issues were reported.

A comma-removal suggestion in the transcript was applied in
about.html. The optional suggestion to remove "actually" was
declined to preserve the spoken wording.