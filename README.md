# PROMPTOPIA

### Promptopia is a Full Stack web application created using Next.js Framework.

### It has CRUD functionalities which allows users to create, read, update and delete their prompts.

### Anyone can use prompts by copying into their clipboards.

## Technical Specifications

`Next.js is a very popular framework which works on the top of react. It has so many powerful features which allows developers to create amazing full stack applications. Every framework created with some set of rules that we need to follow while creating applications.`

`In Next.js routing is very simple and easier as compared to react. Because we just need to create some route folders according to our application requirements.`

`Promptopia allows us to share ideas and create AI Powered prompts which anyone can share and use in AI Platforms to get their work done.`

## Folder Structure

`The Main Entry point of the application is app folder which contains some folder structures and layout for our application to perform routing and creating api endpoints for the application backend.`

`In Backend MongoDB is used to store data related to users and prompts created by users.`

### 1. app

├───api
│ ├───auth
│ │ └───[...nextauth]
│ ├───prompt
│ │ ├───new
│ │ └───[id]
│ └───users
│ └───[id]
│ └───posts
├───create-prompt
├───profile
└───update-prompt

### 2. components

-> Feed.jsx
-> Form.jsx
-> Nav.jsx
-> Profile.jsx
-> PromptCard.jsx
-> Provider.jsx

### 3. models

-> prompt.js
-> user.js

### 4. public

└───assets
├───icons
└───images

### 5. styles

-> globals.css

### 6. Utils

-> database.js

### FUNCTIONALITIES

- [Google Authentication] - By using Google Auth as a client anyone can sign in using their Google account.
  If the account was not found then It will automatically create the user account and save the details in the DB.

- [Prompts Creation] - On Clicking `Create Prompt` users can create their prompts and it will save them to the db.
  we have models created related to prompts which represent the prompt inputs and validation into the database.
  on create prompt we make a `POST` request in our API which we have created in the `api` folder. The path for API is `/api/prompt/new` which makes a secure connection to the database for performing create operation and saving the prompt details.

- [Home Dashboard] - The first page which the user can see is the Home page of Promptopia where the user can see different posts or prompts which are created by users of our application. There are varieties of prompts available to copy and use as your wish. All are AI-powered prompts that help you find and get the task done using AI Tools.

- [Search for prompts] - We have implemented a search functionality where users can type the search keywords like tag names or usernames or any specific word related to a particular prompt or its usage. They will get the required prompts in the form of results.

- [Edit & Delete Prompt] - Any user with a Promptopia account can edit and delete their prompts.
  By clicking on their profile image they will navigate to a profile page, where the user can see their personalized profile with the prompts created by that user, there we provided `edit` and `delete` options to edit and delete particular prompts using the specific promptId.

- [Click on tag] - Prompts have a specific tag associated with them. Which shows the topics or keywords related to the specific prompt. Clicking on a tag will populate the search bar and search related to a specific tag.

- [profile navigation] - By using this functionality anyone can navigate and view different profiles easily.
  when the user clicks on the profile image associated with a particular prompt then it will navigate to that user's profile.

- [Signout user] - We implemented a signout facility for users to securely sign out from Promptopia.

- [View other's profile] - We have implemented the View Profiles option where any user can see other users' profiles on a specific page based on user-id and user search.


## Project Screenshots

### 1. Home Page

![Home Page](https://github.com/yogesh6260/promptopia/assets/75936948/6e9a4158-8569-4160-988a-ba0ab4295593)


### 2. Create Prompt Page

![Create Prompt](https://github.com/yogesh6260/promptopia/assets/75936948/7c7c30e6-3db5-4047-aa1c-489c88280d22)


### 3. User Profile Page

![User Profile](https://github.com/yogesh6260/promptopia/assets/75936948/7d5ec3c5-18c2-4ed7-a9a5-5ec3cd0f04b1)


### 4. Edit Prompt Page

![Edit Prompt](https://github.com/yogesh6260/promptopia/assets/75936948/9de27d13-c015-4c71-8c73-7f3a2c39541b)


### 5. On Search showing prompt cards related to the tag name.

![Search by Tag](https://github.com/yogesh6260/promptopia/assets/75936948/7ebbbca0-710e-467f-a528-1ac91b6aba7c)


### Project Deployment Link -> 
https://promptopia-amber.vercel.app/




