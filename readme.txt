--Readme document for Aaron Lam (aarontl1)--

A reminder on academic integrity, as described in the syllabus.

In general, the course staff expects that you will look at code and examples from many online resources as part of the assignments, particularly to resolve syntax and understand frameworks. We expect that you'll use other libraries you find, and will even require it in some assignments. These practices are often critical to the work of developers today. The best developers are adept at interpreting the examples they see, customizing them to their specific situation, and citing their sources so they can find them later. We expect you to do the same.

While learning from examples is encouraged, attempting to pass an existing project or example from the web as your own is not allowed. If you ever have a question about what is or is not appropriate, feel free to ask the course staff!

Talking to classmates about class material, assignment requirements, etc. is a great way to verify ideas and get feedback. But this distinctly does *not* permit attempting to pass off someone else’s code as your own. Talking over ideas and approaches is allowed, but the work that you produce and submit must be your own.

1. How many assignment points do you believe you completed (replace the *'s with your numbers)?

15/14
- 1/1 Readme
- 3/3 Basic HTML content
- 3/3 Basic CSS styling
- 1/1 Advanced feature
- 3/3 Responsive layout
- 1/1 Passes validation checks
- 3/2 Embraces spirit of the assignment

2. What (a) basic features, (b) CSS features, and (c) advanced features did you include in your portfolio?

(a) Basic features
1) At least one image with alt text.
  - The image of me has an alt image (Aaron Lam)
  - The images used for external links to socials all have alt text (LinkedIn, GitHub, itch.io).
  - Portfolio images have alt text (VR Aliens and Checkers).
  - Images of skills have no alt text since they are descriptive images.
    - Exception to this are the images of the software next to Office skill which I have given alt text to specify each ones.
2) 3 links to external pages (LinkedIn, GitHub, itch.io).
3) 3 pages with navigation between them (index, contact, and projects).
4) Utilized semantic HTML tags (footer and nav).
5) Custom icons from Google Material Icons and Font Awesome

(b) CSS features
1) Modified margins and padding of content.
2) Modified links in various ways (italicize, images, etc.).
2) Modified a lot of colors for many different certain things (current page, resume link, links in footer, etc.).
3) Used custom fonts from Google fonts (with fallbacks) including:
  - Gluten (Google fonts)
  - JetBrains Mono (Google fonts)
  - VT323 (Google fonts)
  - Material Icons (Google fonts) -> webfonts and css/all.css
  - Font Awesome (downloded custom font)
  - Calibri (built-in custom font)
  - sans-serif (last fallback and default sans-serif font)

(c) Advanced features
1) Created a navigation bar that can be used to navigate between the 3 pages I have.
  - Each page has the same navigation bar.
2) Created a table with multipule columns and rows that can be read via a screen reader. 
3) Created a contact form which uses HTML forms in the contact page.
  - Contact form does not actually send (does not have backend implemented).
4) Embededed video of VR Game project with fallbacks.

3. How long, in hours, did it take you to complete this assignment?
Approximately 12-15 hours.

4. What online resources did you consult when completing this assignment? (list specific URLs)
-- Resources for HTML and CSS --
https://www.geeksforgeeks.org/html-tags-complete-reference/
https://www.geeksforgeeks.org/css-properties-complete-reference/

-- Resources for making the contact form --
https://www.w3schools.com/howto/howto_css_contact_form.asp
https://stackoverflow.com/questions/10868640/align-html-input-fields-by
https://stackoverflow.com/questions/1839403/how-do-i-align-a-label-and-a-textarea

-- Custom fonts -- 
https://fonts.google.com/

-- Resources for making the navigation bar --
https://www.w3schools.com/css/css_navbar.asp

-- Used to figure out how to open links to new tabs --
https://www.freecodecamp.org/news/how-to-use-html-to-open-link-in-new-tab/

-- Resources for Font Awesome --
https://fontawesome.com/v5.15/how-to-use/on-the-web/setup/hosting-font-awesome-yourself

-- Inspiration -- 
https://www.freecodecamp.org/news/15-web-developer-portfolios-to-inspire-you-137fb1743cae/

-- favicon -- 
https://favicon.io/favicon-converter/
https://www.hostinger.com/tutorials/how-to-add-favicon-to-website

5. What classmates or other individuals did you consult as part of this assignment? What did you discuss?
- Asked one classmate about submitting the .zip, specifically about whether or not we include the image and media
  files on our webpage in our submission.

6. Is there anything special we need to know in order to run your code?
- Validation checks are in the validation-checks folder
  1) represents index.html and index.css
  2) represents contact.html and contact.css
  3) represents projects.html and project.css
  4) all.css which is the file needed for Font Awesome icons (not sure if I needed to check but did it anyway)
- Validation check for accessibilty has a ngrok link because I used ngrok to host temp URL which I could 
  use to check accessibilty as a whole since just uploading a HTML file does not take to account the 
  styling of the page.
- For making the website responsive, I focused more on the text than the images, video, or contact form.
  - Contact form input looked unwrittable when scaling.
    - Gave it default width and height and made it go to the left for smaller screen sizes.
  - I gave images a default width and height since scaling the images made the images really small which,
    in turn, made the page look slightly worse.