# Blogging Platform

This is a full-stack web application built with React, Node.js, Express, and PostgreSQL that showcases the functionality of a blogging platform. Users can create their own blog posts, explore posts from other users, engage with them by liking and commenting, and manage their profile information.
</br>
The application incorporates various technologies. Redux Toolkit is utilized to store the data of an authenticated user. Cloudinary is used for storing user-uploaded images, such as profile avatars and post images. Requests to the API are handled using React Query, while React Hook Form manages form submissions. For seamless navigation, React Router is employed. Material UI is responsible for styling the application.
</br>

## Features

-   Authentication (login, register, logout)
    -   Authentication system with access tokens sent via cookies.
-   Create and edit blog posts
    -   Preview the blog post before publishing
    -   Upload image to the blog post
-   View the blog posts published by other users
    -   Pagination for blog posts
-   Like and comment on blog posts
-   View the user profile
    -   Update the user profile information
    -   Upload profile avatar
-   Optimistic updates using React Query for enhanced user experience
-   Responsive design for mobile devices
-   Progressive Web App (PWA) support

## Technologies


## Setup

Follow the instructions below to run the application locally.

### Installation

Clone the repository:

```bash
$ git clone https://github.com/ramnathnayak07/blogging-platform.git
```

Install the dependencies:

```bash
# Install the dependencies for the root directory, frontend, and backend
$ cd blog-app-mern/
$ npm run postinstall
```

Run the database migrations and populate the data:

```bash
$ cd backend/
$ npx prisma migrate dev
$ npm run seed
```

Run the application:

```bash
# Run the frontend and backend concurrently
$ cd blogging-platform/
$ npm run dev
```

### Cloudinary Setup

Sign up on [Cloudinary](https://cloudinary.com/) to create an account. Once registered, you can find your API key, API secret, and cloud name in your account settings.

### Environment Variables

Create a `.env` file in the root directory of the project

```bash
$ touch .env
```

Add the following environment variables:

```bash
# PORT to run backend on
PORT=5000
# Connection URL to PostgreSQL database
DATABASE_URL=YOUR_POSTGRES_URL
# Secret key to sign tokens (random string)
TOKEN_SECRET=YOUR_TOKEN_STRING
# Cloudinary configuration
CLOUDINARY_API_KEY=API_KEY
CLOUDINARY_API_SECRET=API_SECRET
CLOUDINARY_CLOUD_NAME=CLOUD_NAME
```
