# Dish of the Day

## What is it?

Dish of the Day is a website which aims to provide an option of recipes to the user that change every day, assisting the user with improving their day-to-day eating habits. This site is aimed at people who wish to change the way they eat at home, but always find themselves stuck in the habit of making the same thing at home without experimenting with other types of food.

The site can be found here: <https://shanebyrne0963.github.io/dish-of-the-day/>

![Dish of the Day displayed on different devices](assets/images/readme/site-display.jpg)

## UI/UX Design

### Color Scheme

- The site is broken down into two color schemes:
  - **White text on gray background** - The header, navigation, footer, course buttons and form use this color scheme.
  - **Black text on white background** - All other instances use this color scheme.
- The color scheme is kept simple to avoid overpowering the images used in the site.

### Typography

- The site uses a single font, Lato, to maintain font style consistency.
- If a certain browser does not support this font, a sans-serif font will be used in it's place.

### Wireframes

- For desktop screen sizes:
  - index.html
    - ![Desktop wireframe for index.html](assets/images/readme/wireframes/desktop-index.jpg)
  - menu.html
    - ![Desktop wireframe for menu.html](assets/images/readme/wireframes/desktop-menu.jpg)
  - Recipe pages
    - ![Desktop wireframe for recipe pages](assets/images/readme/wireframes/desktop-recipe.jpg)
  - Recipe pages with large ingredients list
    - ![Desktop wireframe for large recipe pages](assets/images/readme/wireframes/desktop-recipe-large.jpg)
  - request-recipe.html
    - ![Desktop wireframe for request-recipe.html](assets/images/readme/wireframes/desktop-feedback.jpg)
- For tablet screen sizes:
  - menu.html
    - ![Tablet wireframe for menu.html](assets/images/readme/wireframes/tablet-menu.jpg)
- For mobile screen sizes:
  - index.html
    - ![Mobile wireframe for index.html](assets/images/readme/wireframes/mobile-index.jpg)
  - menu.html
    - ![Mobile wireframe for menu.html](assets/images/readme/wireframes/mobile-menu.jpg)
  - Recipe pages
    - ![Mobile wireframe for recipe pages](assets/images/readme/wireframes/mobile-recipe.jpg)
  - recipe-request.html
    - ![Mobile wireframe for recipe-request.html](assets/images/readme/wireframes/mobile-feedback.jpg)

## Features

### User Interface

- **The Header**

  - The header is a banner situated on top of the webpages consisting of the site name, a slogan that states the purpose of the site
    and a banner image.
  - This is the first piece of information presented to the user upon entering the site, so it is the user's first impression of the site. The header introduces the user with a bright colorful image relating to the website's theme of cooking.

![The header for each page](assets/images/readme/features/header.jpg)

- **The Navigation**

  - Situated at the bottom of the header, the navigation consists of three links to separate internal webpages: Home, Menu and Inspire Us.
  - This segment is vital for quick and easy navigation throughout the website.
  - The Home link takes the user to the main page, so it is positioned to the left of the navigation bar.
  - The Menu link takes the user to the menu of the day page, so it is situated to the right of the Home link.
  - The Inspire Us link takes the user to the recipe request form, which is the least important of the three pages, so it is positioned to the right of the navigation bar.
  - The links are spaced out adequately within the navigation bar to reduce misclicking.

![The navigation bar for each page](assets/images/readme/features/navigation.jpg)

- **The Footer**

  - The footer is the banner that is situated at the bottom of each webpage. It is made up of the social media links and a copyright disclaimer.
  - The social media links are opened in a new tab, so it is best to keep these at the bottom of the page where the user will have experienced all of the page's content.
  - The footer is the main routefor the user to keep in touch with the websire's social media posts.

![The footer for each page](assets/images/readme/features/footer.jpg)

### Content

- **The Home Page**

  - This is the page the user is first presented with upon entering the website. It contains a short description of what the website does and what it's purpose is, accompanied by images of some of the finished recipes the website has to offer.
  - The description is broken up into smaller blocks of text of only 1-2 sentences to make the text easier to read.
  - At the bottom of the page, the user is presented with a button to be taken to the menu page.
  - This page explains how the website works to first time users, and familiar users can use the navigation to go to the menu if they do not wish to read it.

![The home page](assets/images/readme/features/index.jpg)

- **The Menu Page**

  - The menu page is the main focus of the site. The user is presented with 4 separate images representing the meal courses: breakfast, lunch, dinner and dessert.
  - Each image has a heading above it, which expands when clicked on to reveal 3 listed anchors, taking the user to a unique page for each one.
  - These anchors will remain the same every time the page is loaded, and will only refresh at the beginning of the next day.
  - The drop-down menus provide a clean, easy to use user interface to navigate through the different recipes, while minimizing the amount of text on the screen.

![The menu page](assets/images/readme/features/menu.jpg)

- **The Recipe Pages**

  - There are 12 separate recipe pages. Each page consists of an introduction, an image of the finished product, an unordered ingredients list and an ordered method list.
  - Some pages also have a recipe credits line if the recipe was requested by a user through the recipe request form.
  - In terms of HTML structure, all of these pages are exact copies of each other.
  - The steak sandwich is the one exception to the previous point. The ingredients list is spread horizontally as well as vertically, due to the large size of the ingredients list
  - These recipe pages provide the ingredients needed and the cooking process of the dish the user clicked on in the menu.

![The recipe page](assets/images/readme/features/recipe.jpg)

- **The Inspire Us Page**

  - This page allows the user to request a recipe to be made for the website. The user will specify the name of the dish they want and what course it is typically served as.
  - The user is also given an option to give any feedback in relation to the site.
  - The user will be asked to fill out their full name and email address.
  - This page encourages the user to be engaging with the site, and provides valuable information to the site on how to add more recipes to their database.

![The inspire us page](assets/images/readme/features/inspire-us.jpg)

- **The Thank You Page**

  - This is the page the user is taken to after submitting the form. It contains a short thank you paragraph and a short thank you video.
  - The paragraph assures the user that they will be contacted soon with the recipe they are looking for, and encourages them to continue using the menu until then.
  - The thank you video requires to be clicked on to play, encouraging more interaction from the user.
  - This page's main purpose is to give feedback to the user, alerting them that they have submitted the form successfully.

![The thank you page](assets/images/readme/features/thank-you.jpg)

## Testing

### Bugs

1. Image for page description sits underneath the accompanying text

   - Expected result: The image is supposed to share the same vertical space with the text
   - Solution: Using the flexbox layout seemed to be the best fix for this issue. I set the display element of the parent div with id #page-description to flex and everything seemed to work as intended.

2. Menu link button at the bottom of the index.html page overlaps with the elements surrounding it

   - Expected result: The link should have the margins assigned to it
   - Solution: The margins weren't working because the anchor element is an inline element, so the box model couldn't be adjusted. Setting the display property of the #to-menu element to block fixed this issue

3. Setting the overflow to hidden on the course button hid the overflow of the images successfully, but will not allow anything else to display outside the div, such as the collapsible menu underneath.

   - Expected result: The div underneath the image should be visible
   - Solution: Create another div within this div, and set the overflow attribute of the inner div to hidden instead.

4. New dropdown menus don't align properly with their corresponding course button, and they take up 100% of the screen

   - Expected result: Dropdown menus should be the same size as it's parent div
   - Solution: Simple human error. The detail elements' position attributes were set to absolute. However I forgot that when I added the inner div I removed the relative position of the outer div, positioning the details elements in relation to the page instead of the div

5. All text in dropdown menu turns bold when hovered over instead of just the clickable part

   - Expected result: Only the text that's hovered over should be highlighted
   - Solution: Change #daily-menu details:hover to #daily-menu summary:hover

6. Floating image overflows into the footer in recipe page. Div only shapes itself to the list

   - Expected result: Image should have the same height as the list
   - Solution: Using absolute position instead of float works best.

7. For the form, one half lies significantly lower than the other half

   - Expected result: The two halves should be positioned at an equal y coordinate
   - Solution: Absolute positioning fixed this once again

8. All the inputs in the form are in the same position, overlapping each other

   - Expected result: Each input should stack underneath each other
   - Solution: The left and right leaning divs use absolute positioning. The closest parent that has it's position set to relative is the outer form itself. Changing the individual layer's positions to relative should fix this. Also, Having everything within a div use absolute positioning gives the div a size of 0.

9. Cannot click on the dessert radio button because the div height exceeds the height of the form layer

   - Expected result: All radio buttons should be able to be clicked
   - Solution: It seems setting an element's position to absolute removes it from the flow of the webpage, meaning it's size doesn't affect the size of it's parent. The solution I decided on was just to increase the padding for the parent div. It's not the most elegant solution, but everything works properly with this solution (resolved in the following bug fix)

10. The right half of the form is larger than the left half

    - Expected result: Both halves should be the same size and be evenly positioned in the form
    - Solution: Change the form layout from using absolute positioning to grid

11. There is no space between the two columns in the form grid

    - Expected result: There should be a gap separating the two halves of the form
    - Solution: Add a third column of 32 pixels in between the existing columns

12. Image in recipe page overflows out of it's grid cell

    - Expected result: Image should resize itself to fit the grid
    - Solution: Instead of using an img element, set the background image for the grid cell as the image

13. All text in large ingredients recipe reside on one grid cell. This is because I'm setting both the columns and rows for
    the lists at the same time

    - Expected result: Large ingredients lists should share the same row, but not the same column
    - Solution: Add another media query for min-width: 1201px and set the row position for the lists there. This will make it so either the columns or rows will be set but not both

14. Images in index stretch across the page in media query max-width: 1200px

    - Expected result: Images should keep a 1:1 scale, zooming in instead of stretching to fit the given space
    - Solution: Move the description-image class to the span of the image instead of the image itself. Then change the bounding box of the span and set the overflow to hidden

15. Images in index are aligned to the top left in media query max-width: 1200px

    - Expected result: Images should be aligned to the center of the div
    - Solution: Use display: flex in the span for the image, and set the attributes align-items and justify-content to center

16. Error in console: "Failed to load resource: the server responded with a status of 404 ()"

    - Expected result: No errors in console
    - Solution: Adding `<link rel="shortcut icon" href="#">` fixes this issue

17. Flexbox display in index.html expanding divs containing images in FireFox

    - Expected result: FireFox should display the website the same as other browsers
    - Solution: The grid display has shown no issues in other browsers, so I changed the display from flex to grid

### Manual Testing

- **Form Input Validation**
  - First name, last name, email address and recipe name are required in the form and the form will not submit until those fields are filled out.
  - Email address must be valid and the form will not submit until one is given.
  - Only one radio button can be selected for the recipe course, and the form will fail to send if none of them are selected.
  - If the user clicks the submit button and any of these requirements are not met, the user will be given feedback for what needs to be done to complete the form successfully.

![Text input warning](assets/images/readme/testing/input-text.jpg)

![Email input warning](assets/images/readme/testing/input-email.jpg)

- **Anchors**
  - Every link, internal and external, has been clicked on every page and each one works as intended.
  - All external pages are opened in a new tab.
- **Media Queries**
  - Every page has been tested for responsive screen width, with nothing overflowing or overlapping above a screen width of 320px.
- **Other Browsers**
  - I have tested this site on Google Chrome, Microsoft Edge and Mozilla Firefox and confirmed the site works as intended on those platforms

### Validator Testing

- All .html pages have been passed through the [W3C validator](https://validator.w3.org/) and contain no errors or issues ![W3C Validator for index.html](assets/images/readme/testing/w3c-index.jpg)
- The style.css page has been passed through the [Jigsaw W3C](https://jigsaw.w3.org/css-validator/) validator and contains no errors or issues. ![W3C Validator for style.css](assets/images/readme/testing/w3c-css.jpg)
- All foreground and background color combinations have been tested using [WebAIM](https://webaim.org/resources/contrastchecker/) and have all passed. ![WebAIM contrast checker for main content](assets/images/readme/testing/contrast-normal.png)
- All pages have been tested for accessibility using Chrome's lighthouse feature in devtools and I confirmed that the font and text color is easily readable. ![Lighthouse test for index.html](assets/images/readme/testing/lighthouse-index.png)

### Unfixed Bugs

No unfixed bugs.

## Deployment and Local Development

### Deploy on Github Pages

- The site has been successfully deployed to GitHub Pages. The steps to deploy are as follows:
  - In the GitHub repository, navigate to the Settings tab.
  - In the Pages tab, from the source drop-down menu, select "Deploy from a branch".
  - Under the Branch heading, ensure the first drop-down menu has "main" selected and click the "Save" button to the right of it.
  - Wait a few minutes and refresh the page. The link will appear under the GitHub Pages heading.
- The live site can be visited [here](https://shanebyrne0963.github.io/dish-of-the-day/).

### Cloning Repositories

- The site was cloned onto my desktop. The steps to clone are as follows:
  - In the GitHub repository, click on the green button that says "Code". A drop-down menu will appear.
  - In the "Local" tab of the drop-down, there will be a link under the "HTTPS" section. Click the copy button to the right of the link.
  - In the search bar of your PC desktop, search for terminal and open.
  - Type the following command: `git clone https://github.com/ShaneByrne0963/dish-of-the-day.git`.
  - The site will be cloned to your desktop.

### Forking Repositories

- The site was created using a forked repository created by Code Institute. This repository can be found [here](https://github.com/Code-Institute-Org/ci-full-template). The steps to fork are as follows:
  - Navigate to the page of the repository you wish to fork.
  - Click on the green button that says "Use this template". A drop-down will appear underneath, and select "create a new repository"
  - Enter a repository name where specified.
  - Ensure the site is set to public
  - Click "Create repository from template". Codeanywhere will begin to build a new project from that template.

## Credits

### Content

- [Code Institute Full Template](https://github.com/Code-Institute-Org/ci-full-template)
- [Flexbox Tutorial](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [CSS Grid Tutorial](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [Solution to Bug #2](https://forum.freecodecamp.org/t/why-margin-doesnt-work/346366/2)
- [Solution to Bug #15](https://blog.hubspot.com/website/center-an-image-in-html#:~:text=In%20your%20CSS%20code%2C%20find,the%20div%20vertically%20and%20horizontally.)
- [Solution to Bug #16](https://stackoverflow.com/questions/39149846/why-am-i-seeing-a-404-not-found-error-failed-to-load-favicon-ico-when-not-usin)
- [Cookie recipe text](https://joyfoodsunshine.com/the-most-amazing-chocolate-chip-cookies/)

### Media

- Hero image was taken from [Shutterstock](https://shutterstock.com)
- Images for B.L.T and Tuna Melt were taken from [Delish](https://delish.com)
- Image for Bolognese was taken from [Our Table For Seven](https://ourtableforseven.com)
- All other images were taken from [Pexels](https://pexels.com)
- Thank You video was taken from [Envato](https://envato.com)
