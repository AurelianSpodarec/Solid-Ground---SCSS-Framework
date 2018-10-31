# Solid Ground

## Please not that the README needs a heavy re-formatting, as this is the first draft.

A way to manage a robust project with a pragmatic approach, combining methodologies and my experience (not limited), thata promotes consistency, maintanability, scalability and teamwork.

These days you have soo many methodologies and way of doing things. It's just overwhelming. You have BEM, SMACSS, OOCSS, ACSS, ITCC.. WTF?! I like to take big chunks from them and combine.

The key is to understand the concepts behind how to utilize each concept to it's potential.

Note that each project is a unique, and therefroe it requires some sort of customization. The concept and structure I show you, is one that works pretty well for most projects. 

## Table of contents
- [What's Included](#quick-start)
- [What's included](#whats-included)


## What's included

The Solid Ground has the following SCSS directories and files, logically grouping common assets. You'll see something like this:

```
src/
├── assets/
├── js/
└── scss/
    ├── 0-lib/
    |
    ├── 1-helpers/
    |
    ├── 2-settings/
    |
    ├── 3-base/
    |
    ├── 4-layout/
    |
    ├── 5-objects/
    |
    ├── 6-components/
    |
    ├── 7-pages/
    |
    └── styles.scss
```

A quick walkthrough the folders

0-lib: It imports 3rd party code.
1-tools: It help us build the site. Contains code that is mixins, functions, etc.
2-settings: Contains code that is global. Colors, typography config, etc.
3-base: This folder creates the base of the DOM. You have here reset/normalize, global styles for your tag, etc..
4-layout: A place to put things like container, your own grid, anything related to layout. It can also contain components such as heading, footer, the global components.

5-objects: Objects are like small ATOMS. These things form a larger components if put together. It will contains buttons, checkboxes, forms, etc.
6-components: Components are made out of objects. They have a specific use, and they are always made out of smaller componetns first.
7-pages: Specific styles for a page.


## SCSS File Structure

At the top of each file, you can find a # followed by the file name. 
The hash is used to extinquish the file and the classes. Ever wanted to navigate to a file quicky, just to remember that you have hundreds of files and classes to go throguh? That's a waste of time. That's why Using a # is a great way to navigate there quickly.

If the file get's long, add a Table of Content so we can quickly asses where is what in the code and undersand the faster.


## Working with JavaScript the right way

Ever seen a class attribute with 20 classes inside? You have no clue which one is the JavaScript one, or perhaps, how many.

Working with HTML elements using JavaScript is extremelly easy, yet, most developers discard this option.

If you have a JavaScript specific style, you use a data-set attribute. 

When you write it this way, you're telling the developer that this component has something to do with JavaScript, and it's a nice way to divide the styling and the JavaScript in it's own calsses. As class is meant for styling, not for JavaScript hooking.

That is, `data-js` and you're not limited to only that. Make sure they are descriptive. 

Some more examples:

`data-trigger`,
`data-post-id`,
`data-key`,
`data-user`,
`data-date-of-birth`



##Dos and don'ts


### What you probably know

<header></header>

<footer></footer>

<ul></ul>
<ol></ol>
<li></li>

<article></article>


### What you might not know

<figure>
    <img src="pic_trulli.jpg" alt="Trulli" style="width:100%">
    <figcaption>Use semantic tag for text on the image</figcaption>
</figure>

<address>
  James Rockford<br/>
  2354 Pacific Coast Highway<br/>
  California<br/>
  USA<br/>
  +311-555-2368<br/>
  Email: <a href="mailto:j.rockford@example.com">j.rockford@example.com</a><br/>
</address>

<picture>
  <source media="(min-width: 650px)" srcset="img_pink_flowers.jpg">
  <source media="(min-width: 465px)" srcset="img_white_flower.jpg">
  <img src="img_orange_flowers.jpg" alt="Flowers" style="width:auto;">
</picture>

Cite
<img src="img_the_scream.jpg" width="220" height="277" alt="The Scream">
<p><cite>The Scream</cite> by Edward Munch. Painted in 1893.</p>

Blockquote
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 50 years, WWF has been protecting the future of nature. The world's leading conservation organization, WWF works in 100 countries and is supported by 1.2 million members in the United States and close to 5 million globally.
</blockquote>



### Few notes on other elements

The button tag is a 'form' element. The default option for the button is to send a request. Therefore, if you want to use it outside the 'form' element, you must specify the type of the button, to button. This stops the website sending a request to the databse.

<button type="button"></button>


When styling the base of the components, make sure that under any circumstances, you don't touch any global tags, such as the headings, the unorderes/orderes list and so on. That's because if you have a CMS, or if you need the default tag properties, you will need to re-assing/delete whatever there is.

One of my best personal objectives on when to change the global HTML tags is only to reset the entire project to have te project styles. That means if the h1 is meant to be 36px in size, set it. If it meant to have 20px margin bottom, set it. That's where it ends however.


### When to use a button and an anchor tag

I many developers use an anchor tag for a button, with a href that never gets used. 

An anchor tag is used to navigate to another document, to another page if you like. 

If the job is to open a modal for example, we use a button with a type button. You shoudn't use an anchor tag 



### Working WIth JavaScript

One of the biggest issues I face when working on project second hand, is that you get these long classes that are obsqure and you're wondering what is this class. After some time you figiure out that they are there


 

If you feel your project is always on dely or it's messy, this is a place to start.






## If you find your self always doing QA.

## Some tips

### Breaks the project into milestones

### Synchronize work with the desinger


### Weeks of coding can save hours of planning
### Being busy versus being productive

## Collaboration
### Understanding the challenge/problem
### Agreeing on namings and meanings
### Synchronize work with the desinger
### Having one component library
### Object oriented desing & development
### How to report a bug
### Reporting small bugs/issues
### Have small stories. Not big chunks.

## Desing
### Maintaining Desing System
### Approval of components
### Keeping things simple
### Creating a proper Kitchen Sink














 