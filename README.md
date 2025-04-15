# CAPSTONE Programming Project 1 – **Car4All**

Car4All is a modern web application for car sharing and rental services, integrating both back-end logic and front-end interactivity, and using CircleCI for continuous deployment.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Testing](#testing)
- [Contributing](#contributing)
- [License](#license)

---

## Project Overview

**Car4All** is a web-based vehicle booking platform that enables users to view, locate, and reserve available cars within their city using a live interactive map. The system displays real-time car availability by integrating Google Maps with Firebase Firestore, showcasing the power of location-based services.

Key components of the project include:

- A dynamic front-end using Bootstrap and Google Maps API to display available vehicles on a city map.
- Real-time data retrieval from Firebase Firestore to show car information (image, brand, model, seat count).
- Session-based login status management using PHP and browser session storage to toggle navigation options and user account visibility.
- Booking interface allowing users to submit vehicle reservations via form submission.
- Custom header logic that updates based on the user's authentication state.
- A focus on responsive design for mobile and desktop compatibility.

This project serves as a comprehensive showcase of what a full-stack team can achieve in an academic setting, combining design, implementation, and deployment best practices.

---

## Features

- User authentication system (login/register)
- Real-time vehicle availability display
- Interactive Google Maps integration with geolocation
- Location-aware user positioning and navigation
- Vehicle information overlays (images, specs, booking buttons)
- Firebase integration for dynamic backend data
- Responsive front-end design using Bootstrap
- Environment support for both local and CI/CD-deployed builds

---

## Tech Stack

- **Backend**: PHP, Laravel
- **Frontend**: HTML5, CSS3, Bootstrap 3, JavaScript (vanilla)
- **Map & Location Services**: Google Maps API
- **Realtime Database**: Firebase Firestore
- **Deployment/CI**: CircleCI
- **Version Control**: Git, GitHub

---

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/H-Tue-Group-35/CAPSTONE-programming-project-1.git
   cd CAPSTONE-programming-project-1
   ```

2. **Install dependencies**
   ```bash
   composer install
   npm install
   ```

3. **Environment setup**
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```
   - Update `.env` with your database credentials and Firebase configuration.

4. **Run database migrations**
   ```bash
   php artisan migrate
   ```

5. **Start development server**
   ```bash
   php artisan serve
   ```
   - App is now accessible at `http://localhost:8000`

---

## Usage

- Register or login as a user
- View available cars displayed on the map based on real-time availability
- Click on any car to view details and book
- Use geolocation to center the map on your current location
- Navigate to your account or logout using the navbar

---

## Testing

- Ensure PHP and Laravel are properly configured for local development
- Validate map and database integrations using browser developer tools
- Firebase Firestore permissions and rules should be set appropriately

---

## Contributing

We welcome contributions and feedback. Please fork the repository and submit pull requests, or raise issues in the GitHub issue tracker.

---

## License

© 2020 H-Tue-Group-35  
This project is licensed for educational and demonstration purposes.
