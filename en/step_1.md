Google has a free online font library with over 1400 fonts to choose from. The site allows you to browse different fonts using your own sample text to help you find the right one. It then gives you the **HTML** and **CSS** code that you need to **import** the font into your website. 

--- task ---

Open [fonts.google.com](https://fonts.google.com/){:target="_blank"}. It will open in a new tab. 

--- /task ---

--- task ---

Type in some sample text in the **sentence** box:

![A screenshot of the Google fonts search page. The words, Lapsis Sarawack have been placed in the sentence box.](images/custom.png)

**Note** how the examples below now show your sample text. You can see how your words will look in all of the fonts available. 

--- /task ---

There are many different search options to choose from. You can search by category (fallback font families), language or different font properties: 

![A screenshot of the Google fonts search page. The search categories are highlighted.](images/search-options.PNG)

--- task ---

You can scroll down until you find a font you like or, if you know the name of the font, you can type it in the main search box: 

!['Bangers' is typed into the search box.](images/bangers.png)

**Note** that you can now see an example of the Bangers font being applied to the sample text. 

--- /task ---

--- task ---

Click on the card for the font you want to use:

![A screenshot of the Bangers card.](images/bangers-card.PNG)

--- /task ---

--- task ---

Click on the `Select this style` link.

![A screenshot highlighting the 'Select this style' link.](images/select-style.png)

**Note** that a pane will pop in from the side that gives you the code that you need.

--- /task ---

--- task ---

Highlight the HTML text and right click and select copy (tap and hold) to copy the HTML code:

![The HTML text is highlighted.](images/html.png)

--- /task ---

--- task ---

Find the comment in your `index.html` document that says `<!-- Import fonts from Google -->`.

Insert the HTML code that you have just copied below the comment:

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 15
line_highlights: 16-18
---
  <!-- Import fonts from Google -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Bangers&display=swap" rel="stylesheet">

--- /code ---

--- /task ---

You have now imported the fonts that you need from the Google font library. You now need to add in the correct CSS so that the web browser knows when to use this font. 

--- task ---

Go back to the Google font library webpage and copy the CSS code. You only need the code **after** `font-family: `

![The CSS code ''Bangers', cursive;' is highlighted on the Google font library site.](images/css.png)

--- /task ---

--- task ---

Go to your css colour palette file. This will be `default.css` or the file containing the colour palette you have chosen (for example fiesta.css).

Find the `header-font` , `title-font` and `quote-font` variables. 

**Replace** the current fonts` with your new one by deleting the existing text and pressing paste.

--- code ---
---
language: css
filename: default.css
line_numbers: true
line_number_start: 15
line_highlights: 16-17
---
  --body-font: 1.1rem Verdana, sans-serif;
  --header-font: lighter 3rem "Bangers", cursive;
  --title-font: lighter 2rem "Bangers", cursive;
  --quote-font: lighter 1.5rem "Bangers", cursive;

--- /code ---

--- /task ---
