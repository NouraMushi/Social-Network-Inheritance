# Rmotrgram

## Project Description
Rmotrgram is a simple project that simulates a social network similar to Twitter. It allows users to create different types of posts, follow other users, and view a timeline of posts.

## Features

- **User Creation**: Users can create accounts with a first name, last name, and email.
- **Post Creation**: Three types of posts:
  - **TextPost**: A simple text post.
  - **PicturePost**: A post containing text and an image URL.
  - **CheckInPost**: A post containing text and geographic coordinates.
- **Following Users**: Users can follow other users.
- **Timeline**: Displays posts from followed users, sorted from most recent to oldest.

## Class Structure

### Main Classes

1. **User**: Represents a user with:
   - `first_name`
   - `last_name`
   - `email`
   - A list of posts (`posts`)
   - A list of users they follow (`following`)

2. **Post**: Base class for all types of posts, containing:
   - `text`
   - `user`
   - `created_at` (timestamp of creation)

3. **TextPost**: Inherits from `Post` to represent text posts.

4. **PicturePost**: Inherits from `Post` to represent posts containing images.

5. **CheckInPost**: Inherits from `Post` to represent posts with coordinates.
