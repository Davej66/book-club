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



