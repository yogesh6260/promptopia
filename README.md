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

### 6. utils

-> database.js

### FUNCTIONALITIES

- [Google Authentication] - By using Google Auth as a client anyone can signin using their google account.
  If account was not found then It will automatically create the user account and save the details in the DB.

- [Prompts Creation] - On Clicking `Create Prompt` user can create their prompts and it will save to the db.
  we have models created related to prompt which represent the prompt inputs and validation into the database.
  on create prompt we make a `POST` request in our api which we have created in `api` folder. The path for api is `/api/prompt/new` which makes a secure connection to database for performing create operation and save the prompt details.

- [Home Dashboard] - The first page which user can see is Home page of Promptopia where user can see different posts or prompts which are created by users of our application. There are varieties of prompts available to copy and use as your wish. All are AI-powered prompts which helps you find and get the task done using AI Tools.

- [Search for prompts] - We have implemented search functionality where user can type the search keywords like tag names or username or any specific word related to particular prompt or its usage. They will get the required prompts in the form of results.

- [Edit & Delete Prompt] - Any user which has account on Promptopia can edit and delete their prompts.
  By click on their profile image they will navigate to profile page, where user can see their personalize profile with the prompts created by that user, there we provided `edit` and `delete` options to edit and delete particular prompt using the specific promptId.

- [Click on tag] - Prompts have specific tag associated with it. Which shows the topics or keywords related to the specific prompt. By clicking on tag, it will populate to the search bar and search related to specific tag.

- [profile navigation] - By using this functionality anyone can navigate and view different profiles easily.
  when user click on the profile image associated with particular prompt then it will navigate to that user's profile.

- [Signout user] - We implemented signout facility for user to securely signout from Promptopia.

- [View others profile] - We have implemented View Profiles option where any user can see other users profile on a specific page based on userid and user search.


## Project Screenshots

### 1. Home Page

![Home Page](https://github.com/yogesh6260/promptopia/assets/75936948/5d0f8b52-dffe-448a-837d-333fd2ad45aa)

### 2. Create Prompt Page

![Create Prompt Page](https://github.com/yogesh6260/promptopia/assets/75936948/9d103456-bb6e-49de-a9b8-85fcc8fafeec)

### 3. User Profile Page

![User Profile Page](https://github.com/yogesh6260/promptopia/assets/75936948/cff86c83-bc05-40d0-ac11-6429e11ab601)

### 4. Edit Prompt Page

![Edit Prompt Page](https://github.com/yogesh6260/promptopia/assets/75936948/e10bf97c-838e-4cdc-9e50-0be33b4fdc5c)

### 5. On Search showing promptcards related to tag name.

![search by tag](https://github.com/yogesh6260/promptopia/assets/75936948/d8f9116b-6656-42c7-9184-0193f3f756df)



