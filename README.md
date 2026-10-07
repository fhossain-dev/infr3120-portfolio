# Farhan Hossain - Personal Portfolio

INFR3120U Assignment 1: a personal portfolio using HTML5 and CSS3.

## Current progress

- Created four separate HTML pages with shared navigation and footers.
- Added the colour palette, gradients, and responsive stylesheets.
- Added the About-page portrait and HTML5 introduction video.
- Added four project entries with shared card styling.
- Deployment and final validation are still in progress.
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

Testing on the deployed website and formal validation are pending.

## Assistance

AI provided setup guidance and explanations, as well as from course material. 
I adapted the introductory content. Detailed source credits will be
added as the portfolio develops.

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
easy to read, while green highlights navigation interactionS. 

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
All four pages were also checked in Opera browser's responsive preview
at 375 x 800. Navigation, text, and footers fit, and no page errors
were displayed in Console.

Formal HTML, CSS, and accessibility validation is still pending.

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

