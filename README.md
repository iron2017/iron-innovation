Dynamic Chart Application

A web application to dynamically generate and customize charts using the FRED API. Users can search for economic data, visualize it as Line or Bar charts, and customize chart properties.
Features

    Dynamic Chart Rendering: Toggle between Line and Bar charts.
    Search for Economic Data: Fetch data from the FRED API based on user queries.
    Customization Options: Update chart title, type, and color dynamically.
    User-Friendly Interface: Clean and responsive design for an optimal experience.

Technologies Used

    React: Frontend framework for building the application.
    Recharts: Library for creating responsive charts.
    FRED API: Data source for economic statistics.
    Axios: For handling API requests.
    Playwright: End-to-end testing framework.

Getting Started
1. Prerequisites

    Node.js (v14 or higher)
    npm or yarn

2. Installation
unzipe the zip compressed folder
cd dynamic-chart-app

Install dependencies:

    npm install



4. Run the App

    Start the development server:

    npm start or npx vite

    Open the app in your browser at http://localhost:5173.

    second step
    
    move to node-proxy-server
    cd node-proxy-server
    in cmd 
    run node proxyServer.js
    you will get console log thqt the server is running on localhost:5000

Project Structure

src/
│
├── Components/
│   ├── Chart.js              # Chart rendering component
│   ├── ChartManager.js       # Manages chart interactions and API integration
│   └── Header.js             # Application header
│
├── api/
│   └── fredApi.js            # Handles FRED API requests
│
├── styles/
│   └── global.css            # Global inline styles (optional for readability)
│
├── App.js                    # Main application entry
└── index.js                  # Application root

Usage
Search for Data

    Enter a search term (e.g., GDP, Inflation) in the search bar.
    Select a dataset from the results.
    The chart will automatically display the fetched data.

Customize the Chart

    Use the color picker to change the chart’s color.
    Toggle between Line and Bar chart types.
    Update the chart’s title by typing in the input field.

Testing
Run Tests

The application includes automated end-to-end tests using Playwright:

    Install Playwright dependencies:

npm install @playwright/test --save-dev
npx playwright install

Run the tests:

    npm test

Test Cases

    Header rendering
    Chart customization (type, color, and title)
    API data fetching
    Responsive layout verification



