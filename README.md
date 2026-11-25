# Postat

A simple web app that displays random posts fetched from [DummyJSON](https://dummyjson.com), a free fake REST API for testing and prototyping. Users can also search posts by keyword.

**Live demo:** https://assemkaram.github.io/postat/

## Features

- Displays a random post fetched from the DummyJSON API
- Search posts by keyword using the DummyJSON search API

## How It Works

1. The app requests post data from `https://dummyjson.com/posts`. *(Confirm the exact endpoint in `app.js`.)*
2. It picks a random post from the results and renders its title and body.
3. Users can enter a keyword in the search bar to find matching posts.
4. Search requests go to `https://dummyjson.com/posts/search?q=<term>`, and matching results are displayed as a list.

## Getting Started

No build step or dependencies are required.

1. Clone the repository:
   ```bash
   git clone https://github.com/assemkaram/postat.git
   cd postat
   ```
2. Open `index.html` in your browser, or visit the live demo above.

> Fetching data requires an internet connection, since the app calls the DummyJSON API.

## Project Structure

```
postat/
├── index.html   # Page markup, including the search form
├── style.css    # Styles
└── app.js       # Random post loading, search, and rendering
```

## Deployment

The site is hosted with GitHub Pages from the `main` branch.

## Built With

- HTML, CSS, and vanilla JavaScript
- [DummyJSON](https://dummyjson.com) as the data source

