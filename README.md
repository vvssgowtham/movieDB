# Movie Search App

A simple and intuitive movie search application where users can search for movies, explore trending films, and view detailed movie information including ratings, release year, and language.

## Features

- **Search for Movies:** Find movies by title or keyword.
- **Trending Movies:** View the top trending movies currently.
- **Movie Details:** Get details such as rating, release year, and language.
- **Debounced Search:** Optimized search functionality with debounce to prevent excessive API calls.

## Tech Stack

- **Frontend:** React, Tailwind CSS
- **API Integration:** The Movie Database (TMDb)
- **Backend:** Appwrite (for storing search count data)
- **Additional Libraries:** `react-use` for debouncing

## Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/vvssgowtham/movieDB.git
   ```

2. Install the required dependencies:
   ```bash
   cd movieDB
   npm install
   ```

3. Set up environment variables:
   Create a `.env` file in the root directory and add your TMDb API key:
   ```env
   VITE_TMDB_API_KEY = your_tmdb_api_key
   VITE_APPWRITE_PROJECT_ID = your_appwrite_project_id
   VITE_APPWRITE_DATABASE_ID = your_appwrite_database_id
   VITE_APPWRITE_COLLECTION_ID = your_appwrite_collection_id
   
   ```

4. Run the application:
   ```bash
   npm run dev
   ```

5. The app will be available at `http://localhost:5173` (or whichever port your app runs on).

## API Integration

This app fetches movie data from The Movie Database (TMDb) API using the following endpoints:

- **Search Movies:** `GET /search/movie?query={query}`
- **Trending Movies:** `GET /discover/movie?sort_by=popularity.desc`

Ensure that you have the TMDb API key available in your `.env` file as `VITE_TMDB_API_KEY`.

## Contributing

If you'd like to contribute to this project:

1. Fork the repository.
2. Create a new branch for your changes.
3. Make your changes and test them.
4. Submit a pull request.
