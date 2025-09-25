# HomeHive – Rental Listing App
A full-stack rental property web application that allows users to list, view, review, and manage rental properties. Built using Express.js, MongoDB, EJS, Cloudinary, and Mapbox for geolocation.

## Project Structure
```

/models             → Mongoose schemas (Listing, Review, User)
/routes             → Express.js route definitions
/controllers        → Business logic for routes
/public             → Static files (CSS, JS)
/views              → EJS templates for server-side rendering
/utils              → Reusable utility functions
/cloudConfig.js     → Cloudinary image upload config
/app.js             → Entry point of the Express server
```
# Setup
### 1. MongoDB & Cloudinary
Create a MongoDB database (local or MongoDB Atlas)

Create a Cloudinary account for image uploads

Generate a Mapbox token for geocoding

### 2. Environment Variables
Create a .env file in the root:

env
Copy
Edit
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_KEY=your_api_key
CLOUDINARY_SECRET=your_api_secret
MAP_TOKEN=your_mapbox_token
DB_URL=mongodb://localhost:27017/homehive
SECRET=your_session_secret
### 3. Install & Run
```bash

npm install
npm app.js
Runs on http://localhost:3000.
```
# Features
 * Create, read, update, delete property listings

* Upload and store images using Cloudinary

* Location geocoding via Mapbox

* User authentication and authorization

* Leave reviews on listings

* Flash messaging and validations

* Server-side EJS templating



# Notes
 * Ensure .env file is excluded from version control

 * Images are stored in Cloudinary; URLs and filenames are saved in MongoDB

* Uses method-override for HTTP verbs like PUT & DELETE in forms

---
## 🚀 Live Demo

[**View the live application here!**](https://homehive-gzro.onrender.com/listings)
