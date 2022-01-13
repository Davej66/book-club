# **Testing**


### Approach and Tools
As I had deployed my website by my midpoint meeting with my mentor [Richard Wells](https://github.com/D0nni387/) I was in a position to commence testing my website. I was using chrome's web DevTool on every change I made to the website to see the impact and if it met expectations.

Once I had the structure in place, I began testing across other devices screen sizes with chrome's DevTools. Further down the development timeline I also included testing on actual devices; A samsung s20 Ultra, samsung s8, iphone 12 and ipad 4 to complement chrome DevTool.

I also was able to ask family to review the website on their devices for their opinion and issues they encountered.

### Validator Testing
I also used the following to fine tune the process;
 * W3C Markup validator tool for HTML.
   - This has errors caused withe intoduction of jinja to the code. [W3C HTML Validation](https://validator.w3.org/).
 * W3C CSS validator tool for CSS
   - No issues were found with this [W3C CSS Validation](https://jigsaw.w3.org/css-validator/#validate_by_input).
 * PEP8 online for Python
   - No issues were found with this [PEP8 Python Validation](http://pep8online.com/). 
 
 * JSHint (JSHint developer tools) a tool that detects errors and potential problems in JavaScript code.
   - No issues were found with this
 * Lighthouse (chrome developer tools) for security and load times.
   - An issue with the images used from the amazon website, but mongo does not allow large files to be stored which would be incurred with images being stored in the database.       [Chrome Dev Tools (incl Lighthouse)](https://developer.chrome.com/docs/devtools/).


### Bugs and Solutions
#### python method update()
- *Error* - When using the update() method the Werkzeug error was triggered and the error collection is not callable.
- *Fix* - With the guidance of Richard my mentor on how to analysis the error messages we were able to asstain that the version of python used had depreciated the update()                 method and replace_one() was required method.
- *Verdict* - When a book is edited the data is now passed to the database correctly.

#### python method delete()
- *Error* - When using the delete() method the Werkzeug error was triggered and the error collection is not callable.
- *Fix* - With the guidance of Richard my mentor with the previous error above I was able to asstain that the version of python used had depreciated the remove()                 method and delete_one() was required method.
- *Verdict* - When a book is deleted the data is now removed from the database correctly.


## **Client stories testing:**
### **The potential common paths through the website:**

 - Home > Register
 - Home > Log-In
 - Profile > Book
 - Home > Book
 - Book > Shopping Link
 - Book > Edit Book
 - Book > Add a Book
 - Profile > Edit Book
 - Profile > Add a Book

### **As Admin additional functions**

 - Category > Edit Category

Each of these possible paths has been tested repeatedly.

## ** Testing client stories from UX section of README.md **

1. As a first-time visitor, I would like to find a worth reading book.
 - I browse the book list on the home page until I find something interesting, click on the "More Details" button book once found it, read the description and information          provided on the page, click on the " Purchase a copy here " button to head to the store.

2. As a first-time visitor, I would like to find out more about my favourite book and read other readers' reviews.
 - I type the book title in the search box find my favourite book, or
 - Type in the category of my favourite book, scroll the page down to find my intended book.

3. As a first-time visitor, I would like to become a member of a community to be able to add my favourite book to share with the website.
 - I navigate to the sign-up page and create an account, following that I will be navigated to the profile page where I can see the "Add a Book" button on top of the page as        well as in the navigation bar. I enter the requested data into each field and the book I intend will be added to the website and I will be provided with a feedback              message confirming that I have added the book.

4. As a returning visitor, I would like to write a review about a book I have recently read/purchased from the online store.
 - I first log in to my account, then I will look for the book I am looking for. After finding it I scroll down the page until I see the review form, complete the form, and        submit it and a feedback message that a review has been added.

5. As a returning visitor, I would like to delete a review I left on a book.
 - I log in to my account, navigate to my profile page, find the review I am looking for in the list of reviews section and click on the delete button. I will be provided with a    feedback message confirming that the selected review has been deleted.

6. As a returning visitor, I would like to edit a book I added to the website.
 - I log in to my account, navigate to the profile page, scroll down the page until I find the intended book, click on the "Edit" button. I will be navigated to a page with a      pre-filled form with the book details and from there I will be able to modify any field, click on the "Edit button" and a feedback message confirming that I have edited the      book.
 - I log in to my account, type the book title I want to edit in the search box, click on the book, from the book detail page I can see an "Edit" button, I click on that, and      next I will be navigated to a page with a pre-filled form with the book details and from there I will be able to modify any field I want and finally click on the "Edit          button". I will be provided with a feedback message confirming that I Edited the book.

7. As a returning visitor, I would like to Remove a book I added to the website.
 - I log in to my account, navigate to the profile page, scroll down the page until I find the intended book. Click on the "Delete" button and I will be provided with a feedback    message confirming that the book has been deleted.

## ** Manual (logical) testing of all elements and functionality on every page.**
### **Navigation Bar**

- Click on every single link on the navigation bar to assure they are all properly working correctly.
- Check the page URL and make sure it shows the right pathname. [(http://book-club-dj.herokuapp.com/get_books)]
- Check the accessibility to the links that are supposed to be visible on the two different states of logged In/Out.
- Change the screen size from desktop to tablet to verify that the navigation bar is responsive and switches from the inline menu to the burger icon dropdown menu at the           appropriate place.
- Click on the burger icon to make sure the menu opens from the right side of the screen.
- Check the search box size and function on the home page.
- Type a book title that is known it exists and make sure it will be displayed.
- Type an author name and make sure it displays all the books from that author.
- Type a title or an author name that exists in the database and make sure the "No Results found" text displays on the screen.
- Click on the reset button and make sure it resets the searches and displays all books.

### **Home page**

- Resize the window size and make sure that the links have proper position and padding on the iPad and mobile screen.
- Scroll down the page and check the layout of the book cards on the home page.
- Click on the book cards and make sure they navigate to the corresponding book detail page.
- Resize the window in the iPad and mobile screen size to make sure all sections are responsive and the layout changes on different screen sizes.

### **Book Detail page**
- Click on the back button and make sure it returns to the previous home page on the same position.)
- Check the page URL and make sure it shows the right path name as expected and that the book is triggered by its ObjectId. 
  (http://book-club-dj.herokuapp.com/get_book/61defd67924046884ddb972d)]
- Click on the "Purchase a copy here" button and make sure it navigates to the store in a new tab.
- Click on the "Edit" button and make sure it navigates to the edit book page.
- Try to write a review in the review form and submit it when the user is not logged in and make sure it returns to the login page with a feedback message asking the user to       login first.
- Try to submit a review when the user is logged in and make sure that the review is submitted successfully, and a message informing them of the update.
- After submitting a review, scroll down the page and make sure your review is displayed in the review section with correct data.
- Check if the time for the added review is shown and was the correct time.
- Resize the window in the iPad and mobile screen size to make sure all sections are responsive and the layout changes on different screen sizes.

### **Edit Book Page**
- Check the page URL and make sure it shows the right path name as expected and that the book is triggered by its ObjectId to be edited. 
   For instance[(http://book-club-dj.herokuapp.com/edit_book/61df6d0026fd31efbf646070)]
-  Make sure the form is already pre-filled with the book details.
-  Try To change any field from the form and submit the form. Make sure the book is updated as expected and it redirects to the book detail page with the updated data.
-  Try to uncheck the best seller check box and make sure that after the submission the best seller badge is removed from the title.
-	Try to modify any field on the form except the title and make sure it updates the form accordingly.
-  Resize the window in the iPad and mobile screen size to make sure all sections are responsive and the layout changes on different screen sizes.

### **Profile Page**

-	Make sure your account details are displayed correctly on the profile page.
-	Check the page URL and make sure the username is displayed after the profile path. For instance [(http://book-club-dj.herokuapp.com/profile/paula)]
-	Click on the "Edit Profile" button and make sure it navigates to the edit profile page with a pre-filled form with the user's account info.
-	Click on the "Add a Book" button and make sure it navigates to the Add a book page.
-	Scroll down the page and check the list of the books added by the user.
-	Click on the "Edit" button on the added books and make sure it works.
-	Submit the deletion and make sure the feedback message pops up on the page informing the book was deleted.
-	Make sure a "Delete" button is featured on every review added by the user.
-	Check the time of the added review is correct.
-	Click on the "Delete" button on the review section and the right review is deleted. The feedback message pops up on the page informing the review was deleted.
-	Resize the window in the iPad and mobile screen size to make sure all sections are responsive and the layout changes on different screen sizes.

### **Add a Book Page**

-	Click on every single field and make sure they have the applied active style.
-	Try to submit the form with every field empty at a time and make sure it shows the validation error message.
-	Fill out the form accordingly and submit it. Next check if the book is successfully added and with the correct detail and a feedback message informing the book has been          added.
-	Resize the window in the iPad and mobile screen size to make sure all sections are responsive and the layout changes on different screen sizes.

### **Sign In page**

-	Sign Out of the account and make sure the feedback message pops up on the window informing that you have been logged out.
-	Sign out the account and make sure you are navigated to the login page.
-	Click on every field to assure that the active style is applied to the fields and that the labels jump up and make space for the input value.
-	Click on the "Log In" button and make sure you are navigated to your profile page.
-	Check the "Register Account" link underneath the "Log In" button and make sure it navigates to the Sign Up page.
-	Try to log in with an incorrect username and/or password and make sure you won't be logged in and that a feedback message pops up on the window informing that the "Incorrect    Username and/or Password".
-	Resize the window in the iPad and mobile screen size to make sure all sections are responsive and the layout changes on different screen sizes and that the image card won't      be displayed on the mobile screens.

### **Sign In page**

-	Click on every field to assure that the active style is applied to the fields and that the labels jump up and make space for the input value.
-	Try to create an account and leave a field blank to check if the validation error messages pop up.
-	Try to create a username that already exists in the database and make sure a message pops up on the page informing that the username already exists.
-	Try to fill out the form correctly and click on the "Register" button and make sure you are navigated to your profile page with a feedback message informing that you have        registered successfully.
-	Try to create a password and then add a non-matching password in the confirm password field and make sure the error message pops up.
-	Check the "Log In" link underneath the "Register" button and make sure it navigates to the Sign In page.
-	Resize the window in the iPad and mobile screen size to make sure all sections are responsive and the layout changes on different screen sizes and that the image card won't      be displayed on the mobile screen.

### **Sticky back-to-top button**

-	Verify that the button shows up in the right position on every page.
-	Click on the button to confirm that the button works.
-	Open the page in the "Developer Tool", choose a mobile device and ensure that the size and spacing of the button change properly.
-	Click on the button and make sure that the animation effect works properly and the page scrolls to the top smoothly.

### **Footer**

-	Confirm that footer code is identical on all HTML pages.
-	Try to log in and check the footer on every single page to make sure that the links embedded in the footer updates accordingly.
-	Try to log out and check the quick access links in the footer alters according to the navigation bar links on different pages.
-	Resize the window in the iPad and mobile screen size to make sure all sections are responsive and the layout changes on different screen sizes.
-	From the home page, check if all the book collection links are accessible from the footer as well, and check every link separately.

### **Custom 404 Page**

-	Try to change the pathname in the URL manually to a random name and make sure that the custom 404 page appears on the screen informing you that the page is not found.
-	Click on the "Let's Go Home" button and make sure it returns you to the home page.

### **Custom 500 Page**

I have tested the live website on the following browsers and devices;
-	Google Chrome
-	Safari
-	Firefox
-	IE
-	Edge

### **Devices**
-	iPhone X/12 pro (Chrome Developer Tools, On physical devices)
-	Galaxy S21 (Chrome Developer Tools, On physical device)
-	iPad (Chrome Developer Tools, On physical devices)
-	iPad Pro (Chrome Developer Tools)
-	iPad mini (Chrome Developer Tools)

Browser	Issues
Google Chrome	No issues found.
Safari	No issues found
Firefox	No issues found
IE	No issues found
Edge	No issues found

-	All the links and buttons on the website were checked repeatedly.
-	The website has been manually tested and evaluated by my mentor "Richard Wells" and I was provided with valuable feedback and ideas.
-	Friends and acquaintances were asked to review the website, its content, and their user experience.

