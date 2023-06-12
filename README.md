# Dish of the Day

## What is it?

Dish of the Day is a website which aims to provide an option of recipes to the user that change every day, assisting the user with improving their day-to-day eating habits.

## Features

The website features several different webpages, with each one containing a consistent user interface, made up of the following:

### The Header

- The header is a banner situated on top of the webpages consisting of the site name, a slogan that states the purpose of the site
  and a banner image.
- The name and slogan state that the website's main purpose is in relation to cooking.

### The Navigation

- Situated at the bottom of the header, the navigation consists of three links to separate internal webpages: Home, Menu and Inspire Us
- The Home link takes the user to the main page, so it is positioned to the left of the navigation bar
- The Menu link takes the user to the menu of the day page, so it is situated to the right of the Home link
- The Inspire Us link takes the user to the recipe request form, which is the least important of the three pages, so it is positioned to the right of the navigation bar

### The Footer

### The Home Page

- This is the page the user is first presented with upon entering the website.

### The Menu Page

### The Recipe Pages

- There are 12 separate recipe pages. Each page consists of an introduction, an image of the finished product, an unordered ingredients list and an ordered method list.
- Some pages also have a recipe credits line if the recipe was requested by a user through the recipe request form.
- In terms of HTML structure, all of these pages are exact copies of each other, with the exception of the steak sandwich page,

### The Inspire Us Page

### The Thank You Page

- This is the page the user is taken to

## Testing

### Bugs

1. Image is supposed to be beside the first paragraph, but instead sits with the second paragraph

   - Solution: Using the flexbox layout seemed to be the best fix for this issue. I set the display element of the parent div with id #page-description to flex and everything seemed to work as intended.

2. Menu link button at the bottom of the index.html page overlaps with the elements surrounding it

   - Solution: The margins weren't working because the anchor element is an inline element, so the box model couldn't be adjusted. Setting the display property of the #to-menu element to block fixed this issue

3. Setting the overflow to hidden on the course button hid the overflow of the images successfully, but will not allow anything else to display outside the div, such as the collapsible menu underneath.

   - Solution: Create another div within this div, and set the overflow attribute of the inner div to hidden instead.

4. New dropdown menus don't align properly with their corresponding course button, and they take up 100% of the screen

   - Solution: Simple human error. The detail elements' position attributes were set to absolute. However I forgot that when I
     added the inner div I removed the relative position of the outer div, positioning the details elements in relation to
     the page instead of the div

5. All text in dropdown menu turns bold when hovered over instead of just the clickable part

   - Solution: Change #daily-menu details:hover to #daily-menu summary:hover

6. Floating image overflows into the footer in recipe page. Div only shapes itself to the list

   - Solution: Using absolute position instead of float works best.

7. For the form, one half lies significantly lower than the other half
   - Solution: Absolute positioning fixed this once again

### Manual Testing

- Every input in the recipe request form has been tested.
- Every link, internal and external, has been clicked on every page and each one works as intended.
- Every page has been tested for responsive screen width, with

### Validator Testing

- All .html pages have been passed through the W3C validator and contain no errors or issues
- The style.css page has been passed through the Jigsaw W3C validator and contains no errors or issues
- All foreground and background color combinations have been tested using webAIM and have all passed

### Unfixed Bugs

No unfixed bugs.

## Deployment and Local Development

### Deploy on Github Pages

- The site has been successfully uploaded to GitHub Pages and can be visited [here](https://shanebyrne0963.github.io/dish-of-the-day/).

### Cloning Repositories

### Forking Repositories

## Credits

### Content

- [Flexbox Tutorial](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [CSS Grid Tutorial](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [Solution to Bug #2](https://forum.freecodecamp.org/t/why-margin-doesnt-work/346366/2)
- [Solution to Bug #15](https://blog.hubspot.com/website/center-an-image-in-html#:~:text=In%20your%20CSS%20code%2C%20find,the%20div%20vertically%20and%20horizontally.)
- [Solution to Bug #16](https://stackoverflow.com/questions/39149846/why-am-i-seeing-a-404-not-found-error-failed-to-load-favicon-ico-when-not-usin)

### Media

- Hero image was taken from [Shutterstock](https://shutterstock.com)
- Images for B.L.T and Tuna Melt were taken from [Delish](https://delish.com)
- Image for Bolognese was taken from [Our Table For Seven](https://ourtableforseven.com)
- All other images were taken from [Pexels](https://pexels.com)
- Thank You video was taken from [Envato](https://envato.com)
