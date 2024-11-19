# GitHub API Usage Dashboard

## Overview

The **GitHub API Usage Dashboard** is a lightweight web application that helps developers monitor their GitHub API rate limits in real-time. It displays data such as:
- **Total requests allowed** in different API categories (Core, Search, and GraphQL).
- **Remaining requests** before hitting the rate limit.
- **Time until reset** of the rate limits.
- **Your public IP address** for quick reference.

## Features
- **Real-Time Updates**: Automatically refreshes data every 60 seconds.
- **User-Friendly Interface**: Styled with Bulma CSS for a clean and responsive design.
- **Lightweight and Fast**: Built with plain HTML, JavaScript, and CSS—no dependencies or backend required.
- **IP Address Display**: Uses the IPify API to fetch and display your public IP address.

## How It Works
1. Fetches the user's IP address using the [IPify API](https://www.ipify.org/).
2. Fetches GitHub API rate limit data from the [GitHub Rate Limit API](https://docs.github.com/en/rest/rate-limit).
3. Displays the data in an organized and visually appealing layout.
4. Updates the displayed data every minute using `setInterval`.

## Prerequisites
- A web browser with JavaScript enabled.
- Internet connection to access the external APIs.

## Installation and Usage
Option 1
1. Clone or download the repository to your local machine.
2. Open the `index.html` file in a web browser.
3. View your IP address and GitHub API usage details.

Option 2
1. You can also just open the page hosted with GitHub Pages 

No additional setup or dependencies are required.

## Code Explanation
### HTML
The structure of the application is divided into sections:
- **Core API**: Displays information about requests allowed and remaining for the Core API.
- **Search API**: Displays similar details for the Search API.
- **GraphQL API**: Displays details for GraphQL rate limits.

### JavaScript
- Fetches data from:
  - [IPify API](https://api.ipify.org) to get the user's IP address.
  - [GitHub Rate Limit API](https://api.github.com/rate_limit) to retrieve API usage details.
- Parses and formats the API response data for display.
- Updates the data every 60 seconds with `setInterval`.

### CSS
- Uses [Bulma](https://bulma.io/) for responsive and aesthetic styling.
- Customizes sections to make data readable and organized.
