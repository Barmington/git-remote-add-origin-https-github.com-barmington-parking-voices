
 Welcome to parking voice 

Parking Voices is a community platform for road users in the UK to share their experiences, thoughts, and opinions about parking and road-related issues.

The platform gives members of the public an opportunity to share their experiences, interact with an online community, and bring attention to issues they believe deserve visibility.

🔗 Live Demo: https://parking-voices-seven.vercel.app/

Features

* User Authentication: Users can sign up and sign in using Clerk.
* Raise Your Voice: Authenticated users can create and publish posts.
* Amp: Users can give Amp to voices they want to support and increase their visibility.
* Voice of the Day: The voice with the most Amp in the previous 24 hours is displayed at the top of the home page.
* Comments & Nested Replies: Users can comment on posts and participate in discussions through nested replies.
* Category Filtering: Users can filter voices by category.
* Active Voices: Users can view the most recently published voices.
* User Profiles: Users can view and manage their own voices and visit other users’ profiles.
* Post Management: Users can manage and delete their own posts.
* Responsive UI: The application is designed to provide an intuitive experience across different screen sizes.

User Stories

* As a user, I want to view all posts on one page and have a separate page where I can view my own posts.
* As a user, I want to sign up and sign in so that I can interact with the platform and create posts.
* As a user, I want to give Amp to posts and see the Amp count update.
* As a user, I want to comment on individual posts using a dedicated and user-friendly form.
* As a user, I want to reply to comments so that I can participate in discussions.
* As a user, I want to delete my own posts so that I can manage my content.
* As a developer, I want navigation to use redirects and refreshes to provide a smooth user experience.
* As a user, I want the application to be visually appealing and intuitive to use.

Technologies

* JavaScript / TypeScript
* React.js
* Next.js
* Clerk
* Supabase
* Radix UI
* Vercel

Authentication & User Synchronisation

Authentication and user management are handled using Clerk.

Clerk webhooks are used to synchronise user information between Clerk and the application’s database.

* ⁠Clerk Authentication
* ⁠Redirect to Sign In
* ⁠Clerk Webhooks

Database

The application’s database is managed using Supabase.

A database schema was designed to support users, voices, Amp, comments, and related functionality.

Database Schema

Database schema screenshot from Supabase
<img width="814" height="448" alt="dbschema" src="https://github.com/user-attachments/assets/5e3b5f59-4ac9-4e3c-89a5-64b947544401" />


Wireframe

The initial wireframe and design planning were created using Canva.

⁠View Wireframe
https://canva.link/baka8fspo1u3xkn

Resources & References

The project was inspired by the structure of the didit-reddit-upvote-example repository. The application was developed with new code, components, and additional functionality to meet the project’s requirements.

* ⁠Didit Reddit Upvote Example
* ⁠Radix UI


Deployment

The application is deployed using Vercel.

🔗 Live Demo: https://parking-voices-seven.vercel.app/

🔗 GitHub Repository: https://github.com/wnqifw28349/parking-voices


Project Reflections & Challenges

1. Delete Button Permissions

Problem: Users were able to encounter the delete functionality when viewing posts belonging to other users.

Solution: Created a separate delete button and server function and used conditional rendering to ensure users can only delete their own posts.

1. Missing Current User

Problem: Voices and profile pages were not loading when there was no authenticated user.

Solution: Used Clerk’s auth() object to check whether a user was authenticated before attempting to load user-specific information.

1. User Synchronisation

Problem: Newly signed-in users were not being added correctly to the application database.

Solution: Updated the Clerk webhook configuration to ensure user data was synchronised correctly.

1. Database Query Errors

Problem: Some database queries were failing due to connection and undefined-query issues.

Solution: Updated the database connection configuration and tested queries directly in the SQL editor to identify and resolve the issues.

1. Component Variable Errors

Problem: Some variables were undefined between parent and child components.

Solution: Used props to correctly pass the required data between components.

1. Deployment Errors

Problem: The deployed application was experiencing issues related to environment variables and webhooks.

Solution: Updated the required environment variables and webhook configuration to match the production environment.

Project Overview

Parking Voices demonstrates the implementation of authentication, database integration, user-generated content, nested comments, conditional rendering, API/webhook integration, and deployment using modern web development technologies.






