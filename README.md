![image](https://user-images.githubusercontent.com/85559896/148698131-abc16d2a-50d2-46d1-8342-779c84b94399.png)


# **UX User Experience**

## **User Stories**

All pages on this website are responsive to desktop, iPad and, mobile screens. Every effort has been made om making this website to be as intuitive as possible.

- First Time Visitor Goals
- As a First Time Visitor, I want to easily find a book I want to read.
- As a First Time Visitor, I want to be able to easily navigate throughout the site to find content.
- As a First Time Visitor, I want to look for reviews to understand what their users think of them and see if they are trusted.

- Returning Visitor Goals
- As a Returning Visitor, I would like to write a review about a book I have recently read/purchased from the online store.
- As a Returning Visitor, I want to find the best way to get in contact with the organisation with any questions I may have.
- As a Returning Visitor, I would like to edit a book I added to the website.
- As a Returning Visitor, I would like to Remove a book I added to the website.
- As a Returning Visitor, I would like to delete a review I left on a book.


# **Features**

## **Existing Features**

## - Colour Scheme

-o	The font families used in this project are: 
![image](https://user-images.githubusercontent.com/85559896/149192821-a2f27098-c616-4129-bc3b-253c2108b110.png)

The choice of colurs evolved during development.

## - NAV Bar
### - Features
- Menu options available to none members.

![image](https://user-images.githubusercontent.com/85559896/148970586-7ac7e92b-0a29-4b0b-8b14-578906ab9faf.png)

 - Menu options available to members.
 
![image](https://user-images.githubusercontent.com/85559896/148969815-88f50e85-1dbd-42f5-9492-84f229f046f8.png)

- Menu options aviable to admin members.

![image](https://user-images.githubusercontent.com/85559896/148970767-6bde8491-c9b2-41cd-bb9e-dd8ed387b34f.png)



## - Home Page
### - Features
- A search box in which users can search for their favorite books by title, author or category.
- Small book cards with image, title, and author name, which on click navigates users to a page with full information of each book.
- When aa member is logged in the edit and delete buttons are available.

![image](https://user-images.githubusercontent.com/85559896/148966051-24dd836a-8d18-495d-8ad4-d89a7bfbb7ad.png)


## - Profile Page
### - Features

- Book cards with image, bestseller(if selected at adding or editing), category, title, author name, page number and ISBN numbers and purchase link.
- Book description.
- Back button to return to home page.
- If logged in the option to leave a review if not a message suggesting you register.
- Lists any reviews already posted for this book.

![image](https://user-images.githubusercontent.com/85559896/149187911-b065f477-47f0-403f-96ed-b7206d21dd3a.png)

## - Edit Book Page
### - Features

- Book cards with image, bestseller(if selected at adding or editing), title, author name, page number and ISBN numbers and purchase link.
- Edit button sends any amended data to the database, and a message of an updated book.
- Cancel button to return to home page.

![image](https://user-images.githubusercontent.com/85559896/149187496-43797ef4-8b8f-4e27-960f-8408e04557fc.png)

## - Add Book Page
### - Features

- Book cards with image, bestseller(if selected at adding or editing), title, author name, page number and ISBN numbers and purchase link.
- Edit button sends any amended data to the database, and a message of an updated book.
- Cancel button to return to home page.


![image](https://user-images.githubusercontent.com/85559896/148971715-02aec2d6-a8e4-4097-95f7-a78e67575f3b.png)

## - Manage Category Page
### - Features

- Book card category field.
- Edit button sends any you to the category edit page.
- Cancel button to return to home page.

![image](https://user-images.githubusercontent.com/85559896/149223672-065d70ce-5763-4c52-9879-5885f841ddbc.png)

## - Edit Category Page
### - Features

- Book card category input field.
- Edit button sends the new category data to the database.
- Cancel button to return to home page.

![image](https://user-images.githubusercontent.com/85559896/148972538-a9accd4a-b83a-4a4c-a517-9e29335f38cf.png)

## - Login Page
### - Features

- Book card username input field.
- Book card password input field.
- Login button to access member data.
 
![image](https://user-images.githubusercontent.com/85559896/148971976-d390187b-d97f-4184-87c5-9655b59840b3.png)

## - Registration Page
### - Features

- Book card username input field.
- Book card email input field.
- Book card admin access request field.
- Book card password input field.
- Register button to register on a website.
 
![image](https://user-images.githubusercontent.com/85559896/149223522-c83488bd-e279-400e-ae6d-0f3a0629a5eb.png)




## **Yet to be implemented**
1. The addition of an edit user details.
2. The ability to recover access if password forgotten
3. The option to add a user photo or avatar - mongo database restricts storage of large files.
4. To introduce coding to allow a two level membership, member and admin. Currently the new user can request admin rights but only one admin is currently 
   supported by the coding.


# **Techologies Used**

### **Languages**
 * [HTML](https://en.wikipedia.org/wiki/HTML)
 * [CSS](https://en.wikipedia.org/wiki/CSS)
 * [JavaScript](https://en.wikipedia.org/wiki/JavaScript)
 * [Python](https://en.wikipedia.org/wiki/Python_(programming_language))

 ### **Libraries & Framework**
 * [Fontawesome](https://fontawesome.com/) 
 * [Materialize](https://materializecss.com/)
 * [Flask](https://en.wikipedia.org/wiki/Flask_(web_framework))
 * [JQuery](https://en.wikipedia.org/wiki/JQuery)
 
 ### **Tools**
 * [GitHub](https://github.com/)
 * [GitPod](https://gitpod.io/)
 * [Balsamic](https://gitpod.io/)
 * [W3C HTML Validation](https://validator.w3.org/)
 * [W3C CSS Validation](https://jigsaw.w3.org/css-validator/#validate_by_input)
 * [Coolors](https://coolors.co/)
 * [Chrome Dev Tools (incl Lighthouse)](https://developer.chrome.com/docs/devtools/)
 * [Unicorn Revealer (extension on Chrome Development Tools)](https://chrome.google.com/webstore/detail/unicorn-revealer/lmlkphhdlngaicolpmaakfmhplagoaln?hl=en-GB)
 * [JSHint](https://jshint.com/)


## Testing
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


## Deployment

The project after the completed code has been committed and pushed to GitHub can be deployed and [found here.](https://davej66.github.io/dfg/). This is achieved by navigating to the page holding the project repository and executing the following steps:

1. From the menu select **Settings**.
2. Scrolling down the vertical menu (topped by Options) select **Pages** which leads to the **Source section**.
3. Under Source click the drop-down menu labelled None and select Main Branch.
4. You are then required to choose a folder, either Docs or root. You should select root.
5. You can now save these selections and the link to the deployed website will be displayed.
6. The website is live https://davej66.github.io/m2-travelseeker/ .

### To run the project locally:
To achieve this by the following process;
1. Under the repository name and the menu that contains Gitpod click Code.
2. Select HTTPS the location will already be present.
3. To the right of this address is an icon once this clicked the location will be cloned.
4. the clone can be found at this [https://github.com/Davej66/book-club](https://github.com/Davej66/book-club).

## Credits

I have used the following 5 websites to gather inspiration for content.

- https://www.librarything.com/home Book review site
- https://www.w3schools.com/  The up button [the link here to thread to develop this.](https://www.w3schools.com/howto/howto_js_scroll_to_top.asp)
- https://materializecss.com/ Additional features not covered in the course.
- https://www.amazon.co.uk/ Image links were used from this website



## Acknowledgements

Thanking my mentor [Richard Wells](https://github.com/D0nni387/) for his invaluable guidance and continuing support. His input during the mid-review, furthermore at the final review helped me with the project.

Support from the slack community when seeking assistance for the wealth of infomation available.


