# WanderLust 🏕️

**Live Demo:** [https://airbnb-clone-met8.onrender.com](https://airbnb-clone-met8.onrender.com)

WanderLust is a full-stack web application inspired by Airbnb. It allows users to browse, create, edit, and discover beautiful listings (such as homes, apartments, and vacation rentals) around the world.

## 🚀 Features

- **Browse Listings:** View detailed information and photos of available stays.
- **Manage Listings:** Create, edit, and delete your own listings.
- **Interactive Maps:** View listing locations on interactive maps powered by **Mapbox**.
- **Reviews & Ratings:** Users can leave reviews and ratings for listings.
- **User Authentication & Authorization:** Secure login and signup functionality using **Passport.js**.
- **File Uploads:** Upload listing images to the cloud using **Cloudinary** and **Multer**.
- **Form Validations:** Robust server-side validation using **Joi**.
- **Responsive UI:** Clean, modern, and fully responsive user interface built using **EJS** and custom CSS.
- **Flash Messages:** Provides feedback to the user on actions (like creating or deleting listings).
- **Session & Cloud DB:** Session management with **connect-mongo** and cloud database with **MongoDB Atlas**.
- **Error Handling:** Centralized application-level error handling.

## 🛠️ Tech Stack

- **Backend:** Node.js, Express.js
- **Database:** MongoDB, Mongoose, connect-mongo (Session Store)
- **Frontend/Templating:** HTML, CSS, EJS (Embedded JavaScript), ejs-mate
- **Authentication:** Passport.js, passport-local
- **Cloud Storage & Images:** Cloudinary, multer-storage-cloudinary
- **Maps & Geocoding:** Mapbox SDK
- **Other Utilities:** method-override (RESTful routing), Joi (Validation), dotenv (Environment variables), connect-flash

## 📁 Folder Structure

```text
wanderlust/
├── controllers/    # Route controllers (MVC architecture)
├── init/           # Database initialization scripts and sample data
├── models/         # Mongoose models (listing.js, review.js, user.js)
├── public/         # Static assets (CSS, JS, Webpack/Mapbox scripts)
├── routes/         # Express routers (Express Router)
├── utils/          # Utility functions and error handlers (wrapAsync, ExpressError)
├── views/          # EJS templates (layouts, includes, listings, users)
├── app.js          # Main application entry point
├── cloudConfig.js  # Cloudinary configuration
├── middleware.js   # Custom middlewares (auth, validation)
├── package.json    # Project metadata and dependencies
└── schema.js       # Joi validation schemas
```

## ⚙️ Prerequisites

Before running this project locally, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v18+ recommended)
- [MongoDB](https://www.mongodb.com/) (running locally) or MongoDB Atlas URI
- Cloudinary Account (for image uploads)
- Mapbox Account (for maps and geocoding)

## 🚀 Installation & Setup

1. **Clone the repository:**

   ```bash
   git clone <your-repo-url>
   cd wanderlust
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Environment Variables:**
   Create a `.env` file in the root directory and add your credentials:

   ```env
   NODE_ENV=development
   SECRET=your_secret_string
   ATLASDB_URL=your_mongodb_atlas_url
   CLOUD_NAME=your_cloudinary_cloud_name
   CLOUD_API_KEY=your_cloudinary_api_key
   CLOUD_API_SECRET=your_cloudinary_api_secret
   MAP_TOKEN=your_mapbox_public_token
   ```

4. **Initialize the Database:**
   Populate your database with initial sample data (ensure MongoDB is running):

   ```bash
   cd init
   node index.js
   cd ..
   ```

5. **Run the Application:**

   _For Development (using nodemon):_

   ```bash
   npm run dev
   ```

   _For Production:_

   ```bash
   npm start
   ```

6. **Open your browser:**
   Open [http://localhost:8080](http://localhost:8080) (or whichever port is defined in `app.js`).

## ✍️ Author

**Mohd Harish**

## 📄 License

This project is licensed under the [ISC License](LICENSE).
