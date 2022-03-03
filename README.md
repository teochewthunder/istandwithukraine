# istandwithukraine
This generates a graphic in HTML/CSS that can be photographed and used as a profile picture on Social Media.

## HTML
One area is for the image and the other for the dashboard.

The dashboard has two sections. Each section cntrols the formatting of a message. THe messages will show up in the blue and yellow halves of the image, which is styled to look like the Ukranian flag.

- `text1` and `text2` are textboxes that contain the messages.
- `font1` and `font2` are drop-down lists that have a list of font types.
- `size1` and `size2` are range inputs that cntrol font size.
- `bold1` and `bold2` are checkboxes that control if the message is in bold.
- `italic1` and `italic2` are checkboxes that control if the message is in italics.

## CSS
The formatting is mostly aesthetic. The important ones are as follows:
- `top` has a blue background with yellow text and `bottom` has a yellow background with blue text.
- `message1` has the `padding-top` property set so that the text will appear at the bottom of the blue half.

## JavaScript
The `generateGraphic()` function has a parameter, `section`. `section` is either "1" or "2", and helps determine the elements to grab values from. The values will determine text content, size, font, bold and italics.

On pageload, the function is run twice, with "1" and "2" passed in. The function is also run whenever any of the control's values are changed.
