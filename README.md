# Quiet Hacker News

A small Go web application that presents a quiet, minimal list of Hacker News stories.

## Basic functionality

- Loads the current top stories from Hacker News.
- Displays story titles as links to their original articles.
- Shows the hostname for each article.
- Filters out items that are not external story links.
- Fetches story details concurrently to keep page generation responsive.
- Caches results briefly and refreshes them in the background.
- Reports the page rendering time.

## Requirements

- Go 1.16 or later
- Network access to the Hacker News API

## Run

Start the server with the default settings, then open `http://localhost:3000` in a browser.

The server accepts these options:

- `-port`: port for the web server; defaults to `3000`.
- `-num_stories`: number of stories to display; defaults to `30`.

## Tests

Run the test suite with the standard Go test command.