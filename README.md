# Farhan Hossain - Personal Portfolio

INFR3120U Assignment 1: a personal portfolio using HTML5 and CSS3.

## Current progress

- Created the four HTML page files and CSS files.
- Added the initial Home page introduction, navigation, and copyright.
- Styling, the remaining pages, media, and validation are still in progress.

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

