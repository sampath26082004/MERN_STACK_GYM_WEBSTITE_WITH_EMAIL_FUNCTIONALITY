# MERN_STACK_GYM_WEBSTITE_WITH_EMAIL_FUNCTIONALITY
This project is a modern, responsive fitness website built with React and Node.js, featuring sections for services, pricing plans, a contact form, and a BMI calculator to help users on their fitness journey.

# Sweat-Zone Fitness

A modern, responsive fitness website designed to help users on their journey to fitness. This project provides information about fitness plans, a gallery, contact options, and a BMI calculator.

## Table of Contents

* [About The Project](#about-the-project)
* [Features](#features)
* [Technologies Used](#technologies-used)
* [Getting Started](#getting-started)
    * [Prerequisites](#prerequisites)
    * [Installation](#installation)
* [Usage](#usage)
* [Project Structure](#project-structure)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#contact)
* [Acknowledgments](#acknowledgments)

## About The Project

This project aims to provide a comprehensive online presence for a fitness center or personal trainers. It's built with a modern frontend framework to ensure a smooth and interactive user experience. The site includes key sections for showcasing services, engaging with potential clients, and providing useful tools like a BMI calculator.

## Features

* **Responsive Navigation Bar (`<Navbar/>`)**: Provides easy navigation across the site.
* **Hero Section (`<Hero />`)**: An engaging introductory section, likely featuring a call to action like "Let's Get Moving" and "Unleash Your Potential".
* **Gallery Section (`<Gallery />`)**: Showcases various fitness activities and gym environments, potentially with images of people exercising and training.
* **Pricing Plans (`<Pricing />`)**: Displays different fitness packages (e.g., Quarterly, Half-Yearly, Yearly) with details like cost, included equipment, training, and support.
* **Contact Form (`<Contact />`)**: Allows users to send messages via name, email, and message fields.
* **BMI Calculator (`<BMICalculator />`)**: An interactive tool for users to calculate their Body Mass Index by entering height, weight, and gender.
* **Footer (`<Footer />`)**: Contains general information and possibly developer credits.
* **Backend for Email Sending**: Includes a `sendEmail.js` utility, indicating potential server-side functionality for the contact form.

## Technologies Used

* **Frontend**:
    * React.js
    * Vite (as a build tool)
    * HTML, CSS (for styling)
    * React Router (for navigation)
    * `react-toastify` (inferred from `ToastContainer`)
* **Backend**:
    * Node.js
    * Express.js (inferred from `app.js` and `backend` folder structure)
    * `dotenv` (for environment variables, inferred from `config.env`)

## Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

* Node.js (LTS version recommended)
* npm (comes with Node.js) or Yarn

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [(https://github.com/sampath26082004/MERN_STACK_GYM_WEBSTITE_WITH_EMAIL_FUNCTIONALITY.git)]
    ```

2.  **Install Frontend Dependencies:**
    ```bash
    cd frontend
    npm install # or yarn install
    ```

3.  **Install Backend Dependencies:**
    ```bash
    cd ../backend
    npm install # or yarn install
    ```

4.  **Configure Environment Variables (Backend):**
    Create a `.env` file in the `backend` directory and add your environment variables.
    Example `.env`:
    ```
    # For email sending, if applicable
    EMAIL_SERVICE_HOST=your_email_host
    EMAIL_SERVICE_PORT=your_email_port
    EMAIL_USER=your_email
    EMAIL_PASS=your_email_password
    ```

## Usage

To run the project:

1.  **Start the Backend Server:**
    ```bash
    cd backend
    npm start # or node app.js, or a script defined in package.json
    ```

2.  **Start the Frontend Development Server:**
    ```bash
    cd ../frontend
    npm run dev # or yarn dev (as it uses Vite)
    ```

Open your browser and navigate to `http://localhost:5173` (or the port Vite provides) to see the application.

## Project Structure

The project is organized into `frontend` and `backend` directories.
GYM/
├── backend/
│   ├── node_modules/
│   ├── utils/
│   │   └── sendEmail.js         # Email utility using Nodemailer
│   ├── app.js                   # Entry point for backend
│   ├── config.env               # Environment configuration
│   ├── package.json             # Backend dependencies
│   └── package-lock.json
└── frontend/
    ├── node_modules/
    ├── public/
    ├── src/
    │   ├── components/
    │   │   ├── BMICalculator.jsx
    │   │   ├── Contact.jsx
    │   │   ├── Footer.jsx
    │   │   ├── Gallery.jsx
    │   │   ├── Hero.jsx
    │   │   ├── Navbar.jsx
    │   │   ├── Pricing.jsx
    │   │   └── Workout.jsx
    │   ├── App.css
    │   ├── App.jsx
    │   ├── main.jsx
    │   └── index.css
    ├── .gitignore
    ├── eslint.config.js
    ├── index.html
    ├── package.json
    ├── package-lock.json
    └── vite.config.js
