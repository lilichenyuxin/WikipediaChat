# Project WikiChat
A project that aims to add a social flavor over Wikipedia.

## 1. Features

**Authentication**

- Login
- Register
- Protect certain pages to be authenticated user view only

**Core features**

- news submission
  - Submit wikipedia link with ideas
  - Auto parsing Wikipedia content on the backend when user submits
  - Validating URL to ensure it comes from Wikipedia
- news interaction
  - Like news
  - Unlike news
  - Add news to favourite list
  - Remove news from favourite list
  - Add comments
- settings
  - profile updating, nick name and avatar
  - privacy settings
    - set displaying email or not on personal portal
    - set displaying favourites pages or not on personal portal
    - set displaying submitted news or not on personal portal
  - history timeline
    - the favourites list for the current authenticated user
    - the submission news list for the current authenticated user
    - the comments list for the current authenticated user

**Other features:**

- Routes level code splitting
- Share the news to the other social site
- Parsing time as a relative time, like `1 day ago`
- Check user avatar list for all users liked the news
- Check original wikipedia content from the WikiChat news entry
- client side validation when submitting news
- features page
- about page
- FAQ page

## 2. Preview URL

All updates to the `dev` branch will be auto deployed via the CI/CD pipeline

- Project deployment for `dev` update: https://wiki-chat.netlify.app/
  - this one is also populated with data for you get a good overview of the project
  - demo user name: goodboy@goodboy.com
  - demo password: 123
- Storybook deployment for `dev` update: https://wiki-chat-storybook.netlify.app/

## 3. How to run the project

### Start the backend first

0. start local mongodb
1. from the project root
1. `cd backend`
1. `npm ci`
1. `npm run dev`

### Start the frontend

1. from the project root
1. `cd frontend`
1. `npm ci`
1. `npm run start`

> Congrat! Now you are good to go

## 4. Other developer toolings

### To check the Storybook components in isolation

1. from the project root
1. `cd frontend`
1. `npm ci` (if not installed already)
1. `npm run storybook`

### To check the E2E tests suites

1. from the project root
1. `cd frontend`
1. `npm ci` (if not installed already)
1. `npm run cypress:open`: for running tests manually with a nice UI
1. `npm run cypress:run`: for running tests automatically in console
1. Screenshots and video will be saved, check the console for more detail