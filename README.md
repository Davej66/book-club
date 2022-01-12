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
![image](https://user-images.githubusercontent.com/85559896/149192821-a2f27098-c616-4129-bc3b-253c2108b110.png)





## - NAV Bar
![image](https://user-images.githubusercontent.com/85559896/148970586-7ac7e92b-0a29-4b0b-8b14-578906ab9faf.png)

![image](https://user-images.githubusercontent.com/85559896/148969815-88f50e85-1dbd-42f5-9492-84f229f046f8.png)

![image](https://user-images.githubusercontent.com/85559896/148970767-6bde8491-c9b2-41cd-bb9e-dd8ed387b34f.png)


- Features
- A search box in which users can search for their favorite books by title, author or category.
- Small book cards with image, title, and author name, which on click navi

## - Home Page
![image](https://user-images.githubusercontent.com/85559896/148966051-24dd836a-8d18-495d-8ad4-d89a7bfbb7ad.png)

- Features
- A search box in which users can search for their favorite books by title, author or category.
- Small book cards with image, title, and author name, which on click navigates users to a page with full information of each book.





## - Profile Page
![image](https://user-images.githubusercontent.com/85559896/149187911-b065f477-47f0-403f-96ed-b7206d21dd3a.png)



## - Edit Book Page
![image](https://user-images.githubusercontent.com/85559896/149187496-43797ef4-8b8f-4e27-960f-8408e04557fc.png)


## - Add Book Page

![image](https://user-images.githubusercontent.com/85559896/148971715-02aec2d6-a8e4-4097-95f7-a78e67575f3b.png)



## - Manage Category Page
![image](https://user-images.githubusercontent.com/85559896/148972262-ffde7d29-a86c-4cff-9b7f-cabf5f943171.png)

## - Edit Category Page
![image](https://user-images.githubusercontent.com/85559896/148972538-a9accd4a-b83a-4a4c-a517-9e29335f38cf.png)



## - Login Page
![image](https://user-images.githubusercontent.com/85559896/148971976-d390187b-d97f-4184-87c5-9655b59840b3.png)





## **Yet to be implemented**
1. The addition of an edit user details.
2. The ability to recover access if password forgotten
3. The option to add a user photo or avatar - mongo database restricts storage of large files.


# **Techologies Used**

## **Languages**

### Languages
 * [HTML](https://en.wikipedia.org/wiki/HTML)
 * [CSS](https://en.wikipedia.org/wiki/CSS)
 * [JavaScript](https://en.wikipedia.org/wiki/JavaScript)

 ### Libraries
 * [Bootstrap](https://getbootstrap.com/docs/4.5/getting-started/introduction/)
 * [Google fonts](https://fonts.google.com/)
 * [Fontawesome](https://fontawesome.com/)
 * [Google API - maps and places](https://developers.google.com/maps/documentation/places/web-service/overview)
  
 ### Tools
 * [GitHub](https://github.com/)
 * [GitPod](https://gitpod.io/)
 * [Balsamic](https://gitpod.io/)
 * [W3C HTML Validation](https://validator.w3.org/)
 * [W3C CSS Validation](https://jigsaw.w3.org/css-validator/#validate_by_input)
 * [TinyPNG](https://tinypng.com/)
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
  - No issues were found with this [W3C HTML Validation](https://validator.w3.org/).
 * W3C CSS validator tool for CSS
  - No issues were found with this [W3C CSS Validation](https://jigsaw.w3.org/css-validator/#validate_by_input).
 * JSHint (JSHint developer tools) a tool that detects errors and potential problems in JavaScript code.
  - No issues were found with this
 * Lighthouse (chrome developer tools) for security and load times.
  - An issue with the images used from the amazon website. [Chrome Dev Tools (incl Lighthouse)](https://developer.chrome.com/docs/devtools/).

### Bugs and Solutions
#### python method update()
- *Error* - When using the update() method the Werkzeug error was triggered and the error collection is not callable.
- *Fix* - With the guidance of Richard my mentor on how to analysis the error messages we were able to asstain that the version of python used had depreciated the update()                 method and replace() was required method.
- *Verdict* - When a boo is edited the data is now passed to the database correctly.

#### Google Map - viewed on mobile devices
- *Bug* - When the website is viewed on mobile devices google maps is not reponsive. The embed map using iframe returns a "X-Frame-Options' to 'sameorigin'", 
          using comments in stackoverflow there were solutions that required server access or more advanced javascipt/php solutions.
- *Fix* - When reviewing the code and referring to the course and w3schools I used the @media to revise the google map width.
- *Verdict* - The google map is now reponsive in mobile devices.

#### Google Map - standard map markers.


#### Google Map - csp issue.

- *Bug* -The standard map returne after the search also contains markers for businesses and points of interests which could cause the user confusion..
- *Unresolved* - Researching google documentation and other users experience with this and their solutions. 
- *Verdict* -  Continuing to research the possible solution, for this project and future projects implement google API's and depolying them in a website.

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
4. the clone can be found at this [https://github.com/Davej66/m2-travelseeker.git](https://github.com/Davej66/m2-travelseeker.git).

## Credits

I have used the following 5 websites to gather inspiration for content.

- https://www.librarything.com/home Book review site
- https://www.w3schools.com/  [The up buuton](https://www.w3schools.com/howto/howto_js_scroll_to_top.asp)
- https://materializecss.com/ additional features not covered in the course.
- https://www.amazon.co.uk/ Image links were used from this website



## Acknowledgements

Thanking my mentor [Richard Wells](https://github.com/D0nni387/) for his invaluable guidance and continuing support. His input during the mid-review, furthermore at the final review helped me to get project.

Support from the slack community when seeking assistance for the wealth of infomation available.


notes below for use later to be added in a neat format
Code

the up button was found here https://www.w3schools.com/howto/howto_js_scroll_to_top.asp

Problems encountered whendeveloping the site, when using the gitpod environment the update & delete methods were no longer recognised. This was resolved with guidance from mu mentor Richard Wells on analysising the error meesage and identifying tyhat the more recent Python version I was using had depreciated those methods.
