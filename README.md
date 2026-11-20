# Book Discovery

Book Discovery is a responsive website built with vanilla JavaScript, with book data fetched from the [Open Library API](https://openlibrary.org/developers/api).  
Users can explore current trending books, discover books across different genres, view detailed book information and build their own personal library by saving books that interest them.

- [Preview](#preview)
- [Features](#features)
- [Technologies](#technologies)
- [Installation](#installation)
- [What I Learned](#what-i-learned)
- [Challenges](#challenges)
- [Future Improvements](#future-improvements)

## Preview

### Desktop

<p align="center">
  <img src="./assets/screenshots/desktop-dashboard.png" width="400" alt="Book Discovery desktop dashboard">
  <img src="./assets/screenshots/desktop-book-details.png" width="320" alt="Book Discovery desktop book details page">
</p>

### Mobile

<p align="center">
  <img src="./assets/screenshots/mobile-my-library.png" width="150" alt="Book Discovery mobile My Library page">
  <img src="./assets/screenshots/mobile-genre-results.png" width="140" alt="Book Discovery mobile genre results page">
</p>

**Live Demo:**  https://book-discovery-six.vercel.app

**GitHub Repository:**  https://github.com/RidaAli110/Book-Discovery.git

## Features

- **Book Discovery Dashboard:** Explore trending books, discover genres and view the Book of the Day.
- **Book Search:** Search for books by title or author.
- **Trending Books:** Browse a collection of currently trending books.
- **Explore by Genre:** Discover books across different genres, including Mystery, Horror, Adventure and Science Fiction.
- **Book Details:** View book descriptions, authors, topics, page counts, publication dates and publishers.
- **My Library:** Save books to a personal library and filter your saved books by title.
- **Persistent Storage:** Saved books are stored using Local Storage, so they remain available after refreshing the page.
- **Responsive Design:** built using a mobile-first approach to adapt to different screen sizes.
- **Accessibility:** Semantic HTML, accessible labels and keyboard-friendly interactive elements.
- **API Integration:** Fetch book information and cover images from the Open Library API.

## Technologies Used

- HTML5
- CSS3
- JavaScript
- [Open Library API](https://openlibrary.org/developers/api)

## Getting Started

Follow these instructions to run the project locally.

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, etc.).
- Visual Studio Code (or another code editor).
- Live Server extension for VS Code.
- An internet connection to access the Open Library API.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/RidaAli110/Book-Discovery.git
   ```

2. Navigate into the project folder:

   ```bash
   cd Book-Discovery
   ```

3. Open the project in your preferred code editor.

   ```bash
   code .
   ```

4. Start the development server.

## What I Learned

- **API Integration:** I improved my understanding of working with API's by fetching and displaying from the [Open Library API](https://openlibrary.org/developers/api) then using the returned data to get additional book information.
- **Asynchronous JavaScript:** Learned how to use promise.all() when handling multiple API requests and use Caching to reduce repeated API requests.
- **Local Storage:** I became more confident with Local Storage which I initially found challenging. Through this project I learned how to save, retrieve and remove books for the user's personal library.
- **DOM Manipulation:** I practiced how to dynamically create HTML elements using JavaScript to display information retrieved from the API.

## Challenges

- **Preventing Duplicate API Requests:** While fetching author information the requests were repeated since they were being displayed across other pages, so I used Caching with JavaScript Maps to save previously fetched author information so it can be reused when needed.
- **Managing Search State:** I wanted to save filtered search results while navigating to other pages, so I used session storage to save the search term and restore it when the user returns to the My Library page.
- **Handling Different API Response Structures:** Since the API returns responses in different data structures. I had to account for this while accessing properties and displaying fetched book data.

## Future Improvements

- Allow users to add personal book reviews and reading status.
- Recommend books to users based on books saved.
