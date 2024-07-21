# Moonflix

Welcome to Moonflix, an innovative entertainment app developed with the full-stack MERN (MongoDB, Express.js, React.js, Node.js) stack. This app aims to provide users with a seamless and enjoyable experience for discovering and watching their favorite movies and TV shows.

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Setup Instructions](#setup-instructions)
- [API Endpoints](#api-endpoints)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

- **User Authentication**: Secure user authentication using JWT.
- **Movie and TV Show Discovery**: Browse and search for movies and TV shows using data from TheMovieDB.
- **User Profiles**: Personalized profiles to keep track of user preferences.
- **Responsive Design**: Optimized for both desktop and mobile devices.
- **Interactive UI**: Smooth navigation and interaction with Swiper integration.
- **Form Validation**: Robust form handling with Formik and Yup.

## Tech Stack

Moonflix is built using a variety of technologies to ensure a robust and scalable application:

### Frontend

- [Create React App](https://create-react-app.dev/): A quick way to set up a React project with no build configuration.
- [Material UI](https://material-ui.com/): A popular React UI framework for building responsive and attractive user interfaces.
- [React Router](https://reactrouter.com/): Declarative routing for React applications.
- [Formik](https://formik.org/): Form library for handling form state and validation in React.
- [Yup](https://github.com/jquense/yup/): Schema builder for form validation.
- [Axios](https://axios-http.com/): Promise-based HTTP client for making requests to the backend.
- [Swiper](https://swiperjs.com/): Modern touch slider for creating interactive carousels.

### Backend

- [ExpressJS](https://expressjs.com/): Minimal and flexible Node.js web application framework.
- [Mongoose](https://mongoosejs.com/): Elegant MongoDB object modeling for Node.js.
- [Express Validator](https://express-validator.github.io/docs/): A set of express.js middlewares for data validation and sanitization.
- [JWT](https://github.com/auth0/node-jsonwebtoken): Library for generating and verifying JSON Web Tokens.

### APIs

- [TheMovieDB](https://www.themoviedb.org/): An API providing extensive movie, TV show, and actor data.

### Deployment

- Backend: Deployed on Vercel at [Moonflix API](https://moonflix-api.vercel.app/api/v1/).
- Frontend: Deployed on Netlify at [Moonflix Frontend](https://669c86ed9413770381f1e11e--creative-dragon-4beb2d.netlify.app/).

## Setup Instructions

To set up the project locally, follow these steps:

### Prerequisites

Ensure you have the following installed:

- Node.js (v14 or higher)
- npm or yarn
- MongoDB

### Clone the Repository

```bash
https://github.com/Ajaybipul/Entertainment-App/
cd moonflix
```

### Install Dependencies

#### Backend

```bash
cd backend
npm install
```

#### Frontend

```bash
cd frontend
npm install
```

### Environment Variables

Create a `.env` file in the `backend` directory with the following environment variables:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
TMDB_API_KEY=your_themoviedb_api_key
```

### Run the Application

#### Backend

```bash
cd backend
npm start
```

The backend server will run on `http://localhost:5000`.

#### Frontend

```bash
cd frontend
npm start
```

The frontend server will run on `http://localhost:3000`.

## API Endpoints

The backend API provides various endpoints for user authentication, movie data retrieval, and more. Here are some key endpoints:

- **User Authentication**
  - `POST /api/v1/auth/register`: Register a new user.
  - `POST /api/v1/auth/login`: Login a user.

- **Movies**
  - `GET /api/v1/movies/popular`: Get popular movies.
  - `GET /api/v1/movies/:id`: Get movie details by ID.

- **User Profile**
  - `GET /api/v1/profile`: Get user profile data.
  - `PUT /api/v1/profile`: Update user profile data.

For a full list of endpoints, refer to the [API documentation](https://moonflix-api.vercel.app/api/v1/docs).

## Usage

### User Registration and Login

1. **Register**: Navigate to the registration page and fill out the form. Ensure all fields are correctly filled. Formik and Yup handle form validation.
2. **Login**: After registration, use your credentials to log in. A JWT token will be generated and stored in local storage for subsequent authenticated requests.

### Browsing Movies

1. **Home Page**: Browse through the list of popular movies fetched from TheMovieDB.
2. **Search**: Use the search functionality to find specific movies or TV shows.
3. **Details**: Click on a movie or TV show to view detailed information, including cast, crew, and reviews.

### User Profile

1. **View Profile**: Access your profile to view your personal information and preferences.
2. **Update Profile**: Update your profile information as needed. Formik and Yup ensure that all data is validated before submission.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature-name`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/your-feature-name`).
6. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Thank you for using Moonflix! We hope you enjoy discovering new movies and TV shows. If you have any questions or feedback, feel free to open an issue or contact us directly.
