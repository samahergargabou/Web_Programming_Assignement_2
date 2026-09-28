# Web_Programming_Assignement_2


This project uses one HTML page to show two different layouts with separate CSS files.

## Files

- `index.html` contains the six boxes, A through F.
- `styleA.css` arranges them vertically.
- `styleB.css` puts A through E in a row and F in the bottom-right corner.
- `README.md` explains the files and how the layouts work.

## Switching styles

Open `index.html` in a browser. It starts with Style A. To see Style B, change the stylesheet link in `index.html` to:

```html
<link rel="stylesheet" href="styleB.css">
```

Change it back to `styleA.css` to see Style A again. Save the HTML file and refresh the page after each change.

## Challenges

In Style A, I used a Flexbox column with `justify-content: space-between` to spread the boxes over the page. I added a minimum gap and prevented the boxes from shrinking, so a short window scrolls instead of making them overlap. I also used `box-sizing: border-box` on F to keep its black border inside the 100 × 100 pixel box.

The default font line height made the letters sit lower than expected. I set a 40px line height for A–E in Style A and for all the boxes in Style B to keep the text placement consistent with the 10px padding. In Style B, I disabled wrapping and shrinking to keep A–E on one line. I used fixed positioning to keep F 10px from the bottom and right edges of the window when it resizes.
