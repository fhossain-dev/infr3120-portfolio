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

The navigation uses floated list items, each with a width
of 25%. A clearing element after the list keeps the floated
links inside the header. Links have hover and keyboard-focus
styles. No Flexbox is used.

