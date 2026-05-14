# Museum of Candy

The first single-page website that i built to demonstrate fundamental web development skills using HTML, custom CSS, and the Bootstrap 4 framework back then.

## Overview

The Museum of Candy is a landing page. It features:
- A responsive navigation bar that changes color when scrolling.
- A striking hero section with repeating text and imagery.
- Alternating image and text content blocks that stack neatly on smaller screens.

## Technologies Used

- **HTML5**: For the structure and content of the page.
- **CSS3 (Custom)**: To apply specific styles, colors (like the candy-themed pinks and reds), and typography (`app.css`).
- **Bootstrap 4.1.3**: Utilized for its responsive grid system (`row`, `col-lg-6`, etc.), utility classes (`d-none`, `text-center`, `align-items-center`), and pre-styled components like the Navbar.
- **Google Fonts**: The `Nunito` font is used throughout the project for a clean, modern look.
- **jQuery & JavaScript**: Used for the Bootstrap components to function properly (like the mobile navbar toggle) and to add a custom scroll effect to the navbar.

## Project Structure

- `index.html`: The main HTML document containing the page structure and Bootstrap classes.
- `app.css`: The custom stylesheet used to override and add to the Bootstrap defaults, ensuring the unique candy theme.
- `imgs/`: A directory containing the image assets used on the page (e.g., `hand2.png`, `milk.png`, `gumball.png`, etc.).

## How to View

To view the project, simply open the `index.html` file in your preferred web browser. No server setup is required. 

## Features Highlight

- **Responsive Grid**: The layout seamlessly adapts from desktop to mobile screens. On larger screens, text and images sit side-by-side. On mobile, they stack vertically for optimal reading.
- **Dynamic Navbar**: The navigation bar is transparent at the top of the page but transitions to a solid color as you scroll down, ensuring readability against the content.

## Repository Structure


```text
museum-of-candy/
│
├── css/
│   └── app.css          # All custom stylesheets go in a dedicated CSS folder
│
├── imgs/                # All image assets go in a dedicated images folder
│   ├── gumball.png
│   ├── hand2.png
│   ├── lolli_icon.png
│   ├── milk.png
│   └── sprinkles.png
│
├── index.html           # The main entry point of your website must be at the root
└── README.md            # Documentation about your project (this file!)
```

**Explanation of Structure:**
*   **Root Level `index.html`:** GitHub Pages (and most web servers) automatically look for an `index.html` file in the main/root directory to serve as the homepage.
*   **`css/` Folder:** As projects grow, you might have multiple CSS files. Keeping them in a `css` folder keeps your root directory clean. *(Note: If you move `app.css` into a `css` folder, remember to update the link in your HTML to `href="css/app.css"`).*
*   **`imgs/` Folder:** You already did this perfectly! Grouping images prevents your main folder from getting cluttered.
*   **`README.md`:** Always stays in the root directory so it's the first thing people see when they visit your GitHub repo.

## HTML & CSS Fundamentals Cheat Sheet
*(Included as a quick refresher for building websites from scratch without AI)*

### 1. Basic HTML Boilerplate
Every HTML file needs this starting structure:
```html
<!DOCTYPE html>                 <!-- Tells the browser this is an HTML5 document -->
<html lang="en">                <!-- The root element, sets language to English -->
<head>
    <meta charset="UTF-8">      <!-- Character encoding for text -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- For mobile responsiveness -->
    <title>My Website</title>   <!-- The text that appears on the browser tab -->
    
    <!-- Link to your CSS file -->
    <link rel="stylesheet" href="style.css"> 
</head>
<body>
    <!-- All the visible content of your website goes here -->
    <h1>Welcome to My Site</h1>
    <p>This is a paragraph of text.</p>
</body>
</html>
```

### 2. Common HTML Tags
*   `<h1>` to `<h6>`: Headings (H1 is the largest, H6 is the smallest).
*   `<p>`: A standard paragraph of text.
*   `<a>`: An anchor tag used for links. `href` tells it where to go (e.g., `<a href="https://google.com">Google</a>`).
*   `<img>`: An image tag. Requires an `src` (source path) and an `alt` (description for screen readers) (e.g., `<img src="dog.jpg" alt="A cute dog">`).
*   `<div>`: A generic container used to group elements together, usually for styling or layout purposes.
*   `<ul>` and `<li>`: Unordered list (bullet points) and list items.

### 3. Basic CSS Syntax
CSS is used to style the HTML elements. It consists of a **selector** (what you want to style) and a **declaration block** (the styles you want to apply).

```css
/* This is a CSS comment */

/* Styling by HTML Tag */
body {
    background-color: #f4f4f4; /* Sets the background color */
    font-family: Arial, sans-serif; /* Changes the font */
}

/* Styling by Class (starts with a dot . ) */
/* Used for styling multiple elements the same way */
.highlight-text {
    color: red;
    font-weight: bold;
}

/* Styling by ID (starts with a hash # ) */
/* Used for styling ONE unique element on the page */
#main-header {
    text-align: center;
    margin-bottom: 20px;
}
```

---
*Created as a practice project to solidify HTML, CSS, and Bootstrap fundamentals.*
