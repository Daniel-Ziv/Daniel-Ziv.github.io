# Find My Laptop

Welcome to **Find My Laptop**! This web application helps users find the perfect laptop for their needs by asking a few simple questions about their budget, tasks, portability, and more. After users answer these questions, the app suggests laptops based on their preferences.

## Table of Contents

- [Features](#features)
- [Live Demo](#live-demo)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)

## Features

- Dynamic form with multiple questions for gathering user preferences.
- Smart laptop recommendation algorithm based on tasks (gaming, programming, browsing, etc.).
- Budget management that allows users to prioritize price.
- Display of top 5 laptops with a “Show More” option for additional results.
- Animated loading screen while fetching and processing results.
- A user-friendly interface with custom-styled radio buttons and checkboxes.

## Live Demo

Check out the live version of the project at [Live Demo Link](http://daniel-ziv.github.io).

## Installation

To get started with the project locally, follow these steps:

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/find-my-laptop.git
    cd find-my-laptop
    ```

2. **Open the project:**

    Simply open `index.html` in your browser, or use a local server for better experience:

    ```bash
    # If you have Python installed:
    python3 -m http.server
    ```

3. **View in the browser:**

    Open your browser and go to `http://localhost:8000`.

## Usage

1. Once the application is running, you will be greeted with a welcome page.
2. Start by answering a few simple questions:
   - Choose how important price is to you.
   - Select the tasks you will be using the laptop for (e.g., browsing, gaming, programming).
   - Choose your preferred laptop size and portability.
3. The app will process your answers and display the best laptops matching your needs.
4. Click on any laptop result to view more details and purchase options.

### Example Workflow:

- **Step 1:** User selects their budget and how important price is to them.
- **Step 2:** User selects which tasks they need the laptop for.
- **Step 3:** User specifies if laptop size and portability matter.
- **Step 4:** Results are displayed, including a “Show More” option to load additional laptops.

## Project Structure

```bash
├── index.html        # Main HTML file
├── scripts/
│   ├── algo.js       # Laptop recommendation algorithm
│   ├── navigation.js # Navigation between questions
│   ├── sliders.js    # Handle budget slider and form elements
├── styles/
│   ├── sheets.css    # Main CSS file for styling
├── laptops.json      # Mock laptop data file
└── README.md         # This README file
