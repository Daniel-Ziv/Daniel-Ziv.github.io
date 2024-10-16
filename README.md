#Find My Laptop

Welcome to Find My Laptop, a web application designed to help users find the perfect laptop based on their specific needs and preferences. Whether you're a student, gamer, professional, or casual user, our platform guides you through a simple questionnaire to match you with the best laptop options.

Table of Contents

Demo
Features
Getting Started
Prerequisites
Installation
Usage
Project Structure
Data Processing Algorithm
Optimization Techniques
Contributing
License
Acknowledgments
Demo

You can view a live demo of the application here (Replace # with the actual link once deployed).

Features

User-Friendly Questionnaire: An intuitive interface that asks users about their preferences regarding price, tasks, size, and portability.
Real-Time Results: Displays laptop recommendations based on user input, sorted by suitability score.
Loading Spinner: Provides visual feedback while processing data to enhance user experience.
Optimized Performance: Efficient data parsing and sorting algorithms ensure quick loading times.
Responsive Design: The application is fully responsive and works seamlessly on various devices.
Multi-Language Support: Currently available in Hebrew, with potential for additional languages.
Getting Started

Prerequisites
Web Browser: A modern web browser like Chrome, Firefox, or Edge.
Local Server (Optional): For testing purposes, you can use a local server like Live Server for VSCode or http-server via Node.js.
Installation
Clone the Repository
bash
Copy code
git clone https://github.com/yourusername/find-my-laptop.git
Navigate to the Project Directory
bash
Copy code
cd find-my-laptop
Set Up a Local Server
If using VSCode, right-click on index.html and select Open with Live Server.
Alternatively, if you have Node.js installed:
bash
Copy code
npm install -g http-server
http-server
Open the Application
Navigate to http://localhost:8080 (or the port specified by your local server) in your web browser.
Usage

Welcome Screen
Read the introduction and click בואו נתחיל (Let's Start) to begin the questionnaire.
Questionnaire Steps
Price Importance: Indicate how important the price is to you. If price is important, specify your budget range using the slider.
Tasks: Select the tasks you intend to perform with the laptop (e.g., browsing, gaming, programming).
Size Preference: Specify how important the laptop size is and select preferred sizes.
Portability: Indicate how important portability is for you.
Results
After completing the questionnaire, the application will process your input and display the top laptop recommendations.
Each laptop card shows the compatibility percentage, key specifications, and a link to view the product.
Load More Results
If available, click הצג עוד (Show More) to load additional laptop recommendations.
Project Structure

arduino
Copy code
find-my-laptop/
├── index.html
├── sheets.css
├── scripts/
│   ├── sliders.js
│   ├── navigation.js
│   ├── algo.js
├── images/
│   └── (logo and other images)
├── data/
│   └── laptops.json
└── README.md
index.html: The main HTML file containing the structure of the application.
sheets.css: The CSS file for styling the application.
scripts/: Directory containing JavaScript files.
sliders.js: Handles the slider functionalities in the questionnaire.
navigation.js: Manages the navigation between different steps of the questionnaire.
algo.js: Contains the core algorithm for processing user input and ranking laptops.
images/: Contains images used in the application.
data/laptops.json: The dataset of laptops used for recommendations.
Data Processing Algorithm

The core of the application is the algorithm that matches user preferences with laptop specifications.

Key Components
User Preferences: Collected from the questionnaire, including price importance, budget, tasks, size preference, and portability.
Task Weights: Each task has associated weights for different laptop specifications (e.g., RAM size, CPU speed).
Laptop Scoring: Each laptop is scored based on how well it matches the combined weights of the selected tasks and user preferences.
Process Flow
Combine Task Weights: For the selected tasks, their weights are combined to form a unified weight set.
Calculate Laptop Scores: Each laptop is evaluated against the combined weights and user preferences.
Sort Laptops: Laptops are sorted based on their calculated scores in descending order.
Display Results: The top laptops are displayed to the user with their compatibility percentage.
Optimization Techniques

To enhance performance and reduce loading times, several optimization strategies have been implemented:

Data Size Reduction: The laptops.json file is optimized to include only essential data required for processing and display.
Efficient Parsing: Laptop specifications are pre-parsed to minimize redundant computations during scoring.
Optimized Sorting: The sorting algorithm is refined to handle large datasets efficiently.
Limiting Console Logging: Excessive logging is removed to prevent slowing down the application.
Data Structures: Appropriate data structures like objects and maps are used for quick lookups and efficient data handling.
Contributing

Contributions are welcome! If you have ideas for improvements or new features, feel free to open an issue or submit a pull request.

To contribute:

Fork the Repository
bash
Copy code
git fork https://github.com/yourusername/find-my-laptop.git
Create a New Branch
bash
Copy code
git checkout -b feature/your-feature-name
Make Your Changes
Commit Your Changes
bash
Copy code
git commit -am 'Add new feature'
Push to the Branch
bash
Copy code
git push origin feature/your-feature-name
Open a Pull Request
License

This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments

OpenAI's ChatGPT: For providing assistance in code optimization and problem-solving.
Icons8: For the icons used in the application.
Community Contributors: Thanks to everyone who has contributed to improving this project.
Note: To keep the application free, we receive commissions for purchases made through our links.

Contact

For any inquiries or support, please contact:

Email: support@findmylaptop.com
GitHub Issues: https://github.com/yourusername/find-my-laptop/issues
This README was generated to provide a comprehensive overview of the Find My Laptop project. For further details, please refer to the source code and documentation within the repository.






