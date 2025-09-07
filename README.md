# URL Shortner

A lightweight URL shortening service built with Node.js, Express,
MongoDB, and EJS.

------------------------------------------------------------------------

## 🚀 Features

-   Shorten long URLs into compact forms\
-   Redirects through a unique short code\
-   Built using a modular structure (controllers, routes, models,
    services, middleware)\
-   Auto-restarts server during development via `nodemon`

------------------------------------------------------------------------

## 📂 Project Structure

    urlShortner/
    ├── controllers/     # Handles request logic
    ├── middlewares/     # Custom middleware (e.g., validation, auth)
    ├── models/          # Mongoose schemas
    ├── public/          # Static assets (CSS, JS, images)
    ├── routes/          # Express route definitions
    ├── services/        # Business logic (e.g., nanoid generation)
    ├── views/           # EJS templates for rendering UI
    ├── connect.js       # MongoDB connection setup
    ├── server.js        # Entry point to start the app
    ├── package.json     # Project metadata & dependencies
    ├── .env             # Environment variable config (not committed)
    └── .gitignore       # Files and folders to exclude from git

------------------------------------------------------------------------

## 🛠️ Getting Started

### Prerequisites

-   [Node.js](https://nodejs.org/) (v16+ recommended)
-   [MongoDB](https://www.mongodb.com/) (local or Atlas cluster)

### Installation

1.  Clone the repo:

    ``` bash
    git clone https://github.com/chalukyanithin/urlShortner.git
    cd urlShortner
    ```

2.  Install dependencies:

    ``` bash
    npm install
    ```

3.  Set up environment variables:

    -   Create a `.env` file (based on `.env.example`, if available)
        containing:

            PORT=3000
            MONGODB_URI=<your_mongo_connection_string>
            BASE_URL=http://localhost:3000

    -   Replace placeholder values as needed.

4.  Start the server:

    ``` bash
    npm start
    ```

    Your app should now be running at `http://localhost:3000`.

------------------------------------------------------------------------

## 💡 Usage

-   **Shorten a URL:** Send a POST request to `/url` (or as defined in
    your routes) with the long URL in the body.
-   **Access the original:** Visit the generated short link in your
    browser --- e.g., `http://localhost:3000/abcd1234` should redirect
    you to the original URL.

------------------------------------------------------------------------

## ⚙️ Technologies Used

-   **Node.js & Express** -- Backend and routing framework\
-   **MongoDB & Mongoose** -- Database and ORM\
-   **EJS** -- Server-side templating\
-   **nanoid / shortid** -- Generate unique short codes\
-   **dotenv** -- Environment variables management\
-   **nodemon** -- Auto-reload during development

------------------------------------------------------------------------

## 🤝 Contributing

1.  Fork the project\
2.  Create a new branch: `git checkout -b feature-name`\
3.  Commit changes: `git commit -m 'Add some feature'`\
4.  Push to your branch: `git push origin feature-name`\
5.  Open a Pull Request detailing your changes

------------------------------------------------------------------------


## 📧 Contact

-   **Author:** Chilagodu Nithyananda\
-   **Project URL:** <https://github.com/chalukyanithin/urlShortner>
