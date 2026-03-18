# WanderLust 🏕️

WanderLust is a full-stack web application inspired by Airbnb. It allows users to browse, create, edit, and discover beautiful listings (such as homes, apartments, and vacation rentals) around the world.

## 🚀 Features

- **Browse Listings:** View detailed information and photos of available stays.
- **Manage Listings:** Create, edit, and delete your own listings.
- **Form Validations:** Robust server-side validation using **Joi**.
- **Responsive UI:** Clean, modern, and fully responsive user interface built using **EJS** and custom CSS.
- **Error Handling:** Centralized application-level error handling.

## 🛠️ Tech Stack

- **Backend:** Node.js, Express.js
- **Database:** MongoDB, Mongoose
- **Frontend/Templating:** HTML, CSS, EJS (Embedded JavaScript), ejs-mate
- **Other Utilities:** method-override (RESTful routing), Joi (Validation)

## 📁 Folder Structure

```text
wanderlust/
├── init/           # Database initialization scripts and sample data
├── models/         # Mongoose models (e.g., listing.js)
├── public/         # Static assets (CSS, JS)
├── utils/          # Utility functions and error handlers (wrapAsync, ExpressError)
├── views/          # EJS templates (layouts, includes, listings)
├── app.js          # Main application entry point
├── package.json    # Project metadata and dependencies
└── schema.js       # Joi validation schemas
```

## ⚙️ Prerequisites

Before running this project locally, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v18+ recommended)
- [MongoDB](https://www.mongodb.com/) (running locally or a DB URI)

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

3. **Initialize the Database:**
   Populate your database with initial sample data (ensure MongoDB is running):

   ```bash
   cd init
   node index.js
   cd ..
   ```

4. **Run the Application:**

   _For Development (using nodemon):_

   ```bash
   npm run dev
   ```

   _For Production:_

   ```bash
   npm start
   ```

5. **Open your browser:**
   Open [http://localhost:8080](http://localhost:8080) (or whichever port is defined in `app.js`).

## ✍️ Author

**Mohd Harish**

## 📄 License

This project is licensed under the [ISC License](LICENSE).
