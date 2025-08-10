Pokedex - A React & TypeScript Application

A modern Pokedex application built from scratch using React, Redux Toolkit, TypeScript, and SCSS. This project allows users to browse, search, compare, and create a personal collection of Pokémon. The application fetches data from the PokéAPI.

## Features

    Pokémon Info: View detailed information for each Pokémon, including battle stats, types, abilities, and evolution chains.

    Dynamic UI: The UI dynamically picks up the most dominant color from the Pokémon's image and uses it as an accent color.

    Compare Pokémon: Add Pokémon to a comparison queue to see their stats and types side-by-side.

    Personal Collection: Log in with Google (via Firebase Authentication) to save your favorite Pokémon to a personal list stored in Firestore.

    Efficient Searching: A search page that utilizes debouncing to reduce the number of API calls while typing.

    Modern Styling: A sleek, responsive interface styled with SCSS, featuring a glassmorphism effect.

    Notifications: User feedback is provided through toast notifications for actions like adding or removing Pokémon.

## Technologies Used

This project is built with a modern, type-safe stack:

    Core: React, TypeScript, Redux Toolkit

    Styling: SCSS, react-icons

    Routing: react-router-dom

    API & Data: Axios

    Backend & Auth: Firebase (Authentication & Firestore)

    Notifications: react-toastify

## Project Setup & Installation

To run this project locally, follow these steps:

1. Clone the repository:
Bash

git clone https://github.com/your-username/pokedex.git
cd pokedex

2. Install dependencies:
Bash

npm install

3. Set up Firebase:

    Create a new project on the Firebase Console.

    Create a new Web App in your Firebase project.

    In your project settings, find your Firebase configuration object.

    Create a .env file in the root of your project directory and add your Firebase credentials like this:

    REACT_APP_FIREBASE_API_KEY="your-api-key"
    REACT_APP_FIREBASE_AUTH_DOMAIN="your-auth-domain"
    REACT_APP_FIREBASE_PROJECT_ID="your-project-id"
    REACT_APP_FIREBASE_STORAGE_BUCKET="your-storage-bucket"
    REACT_APP_FIREBASE_MESSAGING_SENDER_ID="your-sender-id"
    REACT_APP_FIREBASE_APP_ID="your-app-id"

    Enable Google Authentication in the Firebase Authentication -> Sign-in method tab.

    Set up Firestore Database and ensure the security rules allow reads/writes for authenticated users.

4. Start the development server:
Bash

npm start

The application should now be running on http://localhost:3000.

## Project Structure

The codebase is organized to separate concerns, making it clean and maintainable.

    src/assets: All static assets like images and icons.

    src/components: Reusable React components (e.g., Navbar, Footer, Background).

    src/pages: Top-level page components (e.g., Search, About, MyList).

    src/scss: All SCSS style files, structured to mirror the component hierarchy.

    src/sections: Major layout sections that might contain multiple components.

    src/utils: Utility functions and global TypeScript type definitions.
