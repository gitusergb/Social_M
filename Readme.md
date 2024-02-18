# SOCIO-MASAI

# A Fullstack Social Media App for POSTS

## about Fullstack Social M App     
 - Basic Posts web app built with **React** ,**Express**
 - website where after **login** 
 - one can **create** a post
 - **Edit,Delete** his/her post.
 - All rights reserved by Gauri Bidwai.
 - Copyright &copy; 2024 Social M post App.
          

### Check : https://luxury-cobbler-78396e.netlify.app/

## Getting Started

### OutPut: 

- Front
![Capture 1]()

- SignUp 
![Capture 2]()

- Login
![Capture 3]()

- Users post 
![Capture 4]()

- Create post
![Capture 5]()

- Update post
![Capture 6]()

---

### Prerequisites

Make sure you have Node.js installed on your machine. You can download it from [here](https://nodejs.org/).

### Installation

1. Clone the repository.

   git clone https://github.com/gitusergb/*****

### Backend link :https://social-xbrk.onrender.com/

## Backend
- I had to build an Express application. 
- There are following API endpoints that are present . 
- Also used MongoDB Atlas for this.
- one can read, update, and delete posts only. 

- The following routes are available :
    1. /users/register ==> To register a new user.
    2. /users/login ==> For logging in and generating a token.
    3. /posts ==> This will show my posts.
    4. /posts/add ==> I can add a new post.
    5. /posts/update ==> I can update my posts.
    6. /posts/delete ==> I can delete my posts.
    <br>

Additionally, the following filtering functionalities are available:
1. If the device name is passed as a query, then it will show only those posts from which the post has been made on that device.Means add filter in the code ,create an select tag where user can swich between the device name and according to that should see the posts 
2. For example, device=MOBILE ==> will give me mobile posts only.
3. device1=MOBILE & device2=PC ==> will give me the posts made by mobile and PC.

- used Mongo Atlas for data storage, and for to manage the relationship between posts.
- Middleware is in place, including an authentication middleware to authenticate one for all the restricted routes.
- While coding, followed these practices:
	1. Hashing the password for security.
	2. Using JWT for authentication.
	3. Implementing the MVC (Model-View-Controller) architectural pattern.
	4. Utilizing a .env file for keeping crucial information secure.

---

## Frontend

- They can either use React or just HTML, CSS, and JS for the frontend. The following pages are present:
1. The Home Page
2. The Signup Page
3. The Login Page
4. The Posts Page ==> Only the posts of the user who is currently logged in are visible.With 10 post per page limit
5. There is a delete button for each post, allowing the user to delete a particular post.
6. Along with the delete button, there is an update button as well. Clicking on it takes the user to a form where they can update the post by providing the necessary information. Clicking the ok button updates that particular post.
7. A navbar is always visible, providing easy navigation.
8. A logout button is available, logging the user out and taking them to the posts page where no posts are visible.
9. A counter is situated at the top left corner, showing the number of posts. Once the user logs out, it becomes 0.