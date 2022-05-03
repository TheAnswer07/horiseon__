# Horiseon website code refactor
​
## Table of contents
​
  - [The challenge](#the-challenge)
  - [User Story](#user-story)
  - [Acceptance Criteria](#acceptance-criteria)
  - [Solution](#solution)
  - [Author](#author)
  - [Acknowledgments](#acknowledgments)

​
### The challenge
​
The objective of this challenge is to work with someone else's code (Scout Rule), which recommends to always leave the code a little cleaner than how it initially was making sure that all links are functioning correctly, reworking the CSS file to make it more efficient by consolidating CSS selectors and properties, organizing them to follow the semantic structure of the HTML elements, and including comments before each element or section of the page.
​
### User Story
​
•	AS A marketing agency
•	I WANT a codebase that follows accessibility standards
•	SO THAT our own site is optimized for search engines

​
### Acceptance Criteria
​
•	GIVEN a webpage meets accessibility standards
•	WHEN I view the source code
•	THEN I find semantic HTML elements
•	WHEN I view the structure of the HTML elements
•	THEN I find that the elements follow a logical structure independent of styling and positioning
•	WHEN I view the image elements
•	THEN I find accessible alt attributes
•	WHEN I view the heading attributes
•	THEN they fall in sequential order
•	WHEN I view the title element
•	THEN I find a concise, descriptive title

​
### Solution

•	HTML changes:

1.	Updated the website's name/title from "website to "Horiseon website"

  <title>Horiseon website</title>


2.	Changed the first div of the body into “header”

    <header>
        <h1>Hori<span class="seo">seo</span>n</h1>


3.	Changed this div into "nav" with class=”main-nav”

<nav class=”main-nav”>

4.	Class "main" created to replace "hero" to be more meaningful regarding the main image

<nav class=”main-nav”>

5.	Class "main" created to replace "hero" to be more meaningful regarding the main image

    <main class="main"></main>

6.	Class “solutions” added to the section ”content" in order to replace class="search-engine optimization", class="online-reputation-management", class="social-media-marketing" and got rid of the extra class

<section class="content">
        <div class="solutions">

7.	Created id="search-engine-optimization", id="online-reputation-management" and id="online-reputation-management" in order to target them to scroll to their respective sections on the website when clicked on from the navbar.

<div class="solutions" id="search-engine-optimization">

<div class="solutions" id="online-reputation-management">

<div class="solutions" id="social-media-marketing">


8.	Class “advantages” added to the section ”benefits" in order to replace class="benefit-lead", class="benefit-brand", class="benefit-cost" and got rid of the extra class

<section class="benefits">
        <div class="advantages">

9.	Changed the div for the footer into just “footer”

<footer>
        <h2>Made with ❤️️ by Horiseon</h2>
            <p>
            &copy; 2019 Horiseon Social Solution Services, Inc.
            </p>
    </footer>


•	CSS changes:

1.	“nav” targeted instead of the initial "div" that it was

header nav {
    padding-top: 15px;
    margin-right: 20px;
    float: right;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 20px;
}

2.	“nav” targeted instead of the initial "div" that it was
header nav {
    padding-top: 15px;
    margin-right: 20px;
    float: right;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 20px;
}

3.	Only targeted the “li” via the new nav and got rid of the remaining elements -div ul - in css

nav li {
    list-style-type: none;
    display: inline-block;
    margin-left: 25px;
}

4.	Added margin-top: 20px and text-align: left to all paragraphs

p {
    font-size: 16px;
    margin-top: 20px;
    text-align: left;
}

5.	Added margin-top: 20px and text-align: left to all paragraphs

p {
    font-size: 16px;
    margin-top: 20px;
    text-align: left;
}


6.	Added padding-bottom: 20px to "main"

.main {
    …
    padding-bottom: 20px;
}


7.	Class “advantages” targeted to reduce the amount of code | Added “text-align: center” for aesthetics

.advantages {
    margin-bottom: 32px;
    color: #ffffff;
    text-align: center;
}


8.	“img” targeted thanks to class “advantages” to reduce the amount of code

.advantages img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}

9.	Class “solutions” targeted to reduce the amount of code

.solutions {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}

10.	“img” targeted thanks to class “solutions” to reduce the amount of code

.solutions img {
    max-height: 200px;
}


​
### Links
​
- Solution URL: git@github.com:TheAnswer07/horiseon.git
- Live Site URL: file:///Users/md/Desktop/bootcamp/homework/horiseon/index.html#social-media-marketingcom)
​
## My process
​
### Built with
​
- HTML5
- CSS
​
## Author
​
Moussa Dia
​
​
## Acknowledgments
​
I worked with my cohort Jack Youkstetter for 15 minutes reviewing and polishing part of this code. It was a great and appreciated collaboration.