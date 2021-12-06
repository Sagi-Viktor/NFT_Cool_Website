# NFT_Cool_Website

## Story

It is time to make money.
Have you ever wondered what is NFT, well long story short NFT is a non-fungible token stored in the blockchain.
And your task is to implement a web page for the Shinie New NFT Collection launches soon.

The initial version of the site must be able to handle huge trafic and etc.
There is no need for additional functionality, such as online shop-center or comments and answers.

## What are you going to learn?

- Create a Flask project.
- Use routes with Flask.
- Use HTML and the Jinja templating engine.
- SQL datamanagemant.
- Use CSS
- Learn "Web Page Asthetic"

## Tasks

1. Implement the `/main` page that displays all fist class information.
    - The page is available under `/main`.
    - The data is loaded and displayed from SQL files.

2. Create the `/frequently-questioned-answers` page that displays a question and the answers for it.
    - The page is available under `/frequently-questioned-answers`.
    - The page displays the question title and message.
    - The page display the answer to a question.

3. Implement a form that allows the user to login.
    - There is an `/login` page with a form.
    - The page is linked from the navbar.
    - There is a POST form with at least `username` and `password` fields.
    - After submitting, the page redirects to the `/user/<user_id>` profile page.

4. Implement a form that allows the user to Registrate.
    - There is an `/registration` page with a form.
    - The page is linked from the navbar.
    - There is a POST form with at least `username`, `password` and `do you want email notifications chechbox` fields.
    - After submitting, the page redirects to the main page.

5. Implement deleting subscription.
    - There is a deletion link on the profile page.
    - Deleting is implemented by the `/user/<user_id>/delete-sub` endpoint.
    - Deleting redirects to the list of questions.

6. Implement the gallery.
    - There is an `/nft-galery` page with a form.
    - The page is linked from the navbar.
    - There is a GET form with sorting fields.
    - After submitting, the page reload it self with query parameters.

7. Implement a the `navbar`.
    - There is "menu" on the top of the page.
    - The navbar can redirect the user to pages like `home` with a logo, `gallery`, `about this project`, `login`, `registration`.
    - After clicking on the navbar, the page redirects to the specic page.

8. Implement editing an existing question.
    - There is a `/question/<question_id>/edit` page.
    - The page is linked from the question page.
    - There is a POST form with at least `title` and `message` fields.
    - The fields are pre-filled with existing question data.
    - After submitting, the page redirects to the "Display a question" page. The changed data is visible on the "Display a question" page.

9. Implement a `footer`.
    - There is a `footer` at the bottom of the page.
    - The rest is be in charge of your own imegination.

10. Create a well recogniaziable easy for the eye design.
    - The same design rules applied to all of the pages.
    - Try to use dark color in contrast of the NFTs.
    - Use as few colors as possible, only the NFT is the point of the site not the site it self.

## General requirements

- A fully functonal well designed site.

## Hints

 ### Project structure

- Split the code into modules according to clean code principles.
- Do not put more than 100-150 lines of code into a single file.
- Make sure that files logically contain the same things. For example,
you can split the code into the following 3+1 parts.

**Layer** | **Example filename** | **What should it do/contain?**
---|---|---
Routing layer | `server.py` | This layer contains logic related to Flask, such as server, routes, request handling, session, and so on. This is the only file to be imported from Flask.
Persistence layer | `data_manager.py` | This is the layer between the server and the data. Functions here are called from `server.py` and use generic functions from `connection.py`.
SQL connection layer |  `connection.py` | This layer contains common functions to execute SQL files without feature-specific knowledge. Only this layer can access long term data storage.
- Utility "layer" | `util.py` | Helper functions that can be called from any other layer, but mainly from the business logic layer.

This is just one way to structure code, you do not have to follow it _strictly_.

### Data models

- Discuss this later on, when the project started

## Background materials

- <i class="far fa-exclamation"></i> [CSS Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- <i class="far fa-exclamation"></i> [CSS Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)


### Feel free to add useful background materials here. ^^^^
