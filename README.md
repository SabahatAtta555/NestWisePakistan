### Full-Stack Development

NestWise Pakistan was developed as a complete **full-stack web application** with a React.js frontend, Python/Flask backend, REST APIs, database integration, authentication, external API integration, Docker containerization, and an automated CI/CD pipeline.

### Frontend Development

* **React.js** – Used to build the complete interactive user interface.
* **JavaScript** – Used for application logic, API requests, filtering, forms, recommendation interactions, authentication handling, and dynamic content.
* **HTML5 & CSS3** – Used for page structure, responsive layouts, property cards, forms, navigation, dashboards, and mobile-friendly design.
* **Vite** – Used as the React development and production build tool.
* **Responsive Design** – The interface is designed for desktop, laptop, tablet, and mobile devices.

The React frontend includes:

* Home page
* User login/signup
* Property search
* Houses for rent
* Houses for sale
* Hostel listings
* Hotel listings
* AI/property recommendation agent
* Property details
* Favorites
* User inquiries
* Property website links
* Buy/Rent filters
* City and area filters
* Budget filters

### Backend Development

* **Python** – Used for backend application development and business logic.
* **Flask** – Used to create the backend server and REST API.
* **Flask REST API** – Connects the React frontend with the server and database.

The Flask backend handles:

* User authentication
* Property data
* Property search
* Filtering
* Recommendation requests
* Favorites
* Customer inquiries
* Buy/Rent property information
* House sale prices
* Hostel and hotel information
* External property websites
* Database operations
* API responses
* Error handling

### REST API Architecture

The frontend and backend communicate through **REST APIs**.

Architecture:

React.js Frontend
→ HTTP/JSON Requests
→ Flask REST API
→ Application Logic
→ SQLite Database
→ JSON Response
→ React.js Interface

Example operations include:

* `GET` property listings
* `GET` houses for sale
* `GET` rental properties
* `POST` login/signup
* `POST` recommendation requirements
* `POST` property inquiries
* `POST` favorites
* `DELETE` favorites
* Search and filter API requests

### Database

* **SQLite** – Used as the relational database for persistent project data.

The database stores information such as:

* Users
* Houses
* Apartments
* Hostels
* Hotels
* Rental prices
* House sale prices
* Cities
* Areas
* Bedrooms
* Bathrooms
* Property size
* Amenities
* Favorites
* Inquiries
* Property website information
* Seller/agency information

The project currently includes demo properties across multiple Pakistani cities.

### Authentication & Security

* **JWT – JSON Web Token** authentication is used for secure user sessions.
* Passwords are hashed instead of being stored as plain text.
* Protected backend routes require authentication.
* User input is validated by the backend.
* Environment variables are used for configuration and sensitive values.

Authentication flow:

User Login
→ React sends credentials
→ Flask verifies credentials
→ Backend generates JWT
→ React stores authentication state
→ JWT is sent with protected API requests

### Property Recommendation Agent

The project includes a smart recommendation agent that receives user requirements such as:

* City
* Preferred area
* Budget
* Rent or purchase
* House / hostel / hotel
* Number of bedrooms
* Family/student/work requirements
* Property size
* Furnishing
* Parking
* Security
* Wi-Fi
* Kitchen
* Laundry
* Nearby facilities

The backend compares these requirements with available property data and ranks suitable options.

The system also explains why a recommended property matches the user's requirements.

### Buy & Sell Property System

The application supports both **property rental and house purchasing**.

For houses for sale, the system handles:

* Total property price
* Lakh/Crore price formatting
* Marla
* Kanal
* Square yards
* Bedrooms
* Bathrooms
* Location
* Seller type
* Agency/source
* Property website
* Purchase budget
* Buyer inquiry

### API Integration

External APIs are integrated to provide additional location information.

* **OpenStreetMap**
* **Overpass API**
* Location/geographical services

These can provide nearby information such as:

* Hospitals
* Universities
* Restaurants
* Pharmacies
* Shops
* Transport locations
* Important surrounding facilities

The property listing prices remain clearly separated from live external map data when demo information is being used.

### Docker

* **Docker** is used to containerize the application.
* Separate frontend and backend environments can run consistently across different computers.

Docker helps package:

* React frontend
* Python/Flask backend
* Required dependencies
* Application configuration

### Docker Compose

* **Docker Compose** is used to manage multiple application services together.

Instead of manually starting each service, the complete project can be started using:

`docker compose up --build`

Docker Compose coordinates the frontend and backend services.

### Git & GitHub

* **Git** is used for source-code version control.
* **GitHub** is used to host and manage the project repository.

Git is used for:

* Tracking code changes
* Commits
* Version history
* Branch management
* Collaboration
* CI/CD triggers

### GitHub Actions

**GitHub Actions** is used to automate the development pipeline.

Whenever code is pushed to GitHub, the workflow can automatically:

1. Checkout the latest source code
2. Set up Python
3. Install backend dependencies
4. Validate the Flask backend
5. Run backend/API tests
6. Set up Node.js
7. Install React dependencies
8. Build the React production application
9. Validate Docker configuration
10. Build Docker containers
11. Generate deployment artifacts

### CI/CD Pipeline

A complete **Continuous Integration / Continuous Delivery pipeline** is included.

Pipeline flow:

Developer Push
→ GitHub Repository
→ GitHub Actions
→ Backend CI
→ API Tests
→ Frontend CI
→ React Production Build
→ Docker Validation
→ Docker Build
→ Deployment Artifact
→ Deployment

**Continuous Integration (CI)** verifies that new code works correctly before deployment.

**Continuous Delivery/Deployment (CD)** prepares successful versions of the application for deployment automatically.

### DevOps

DevOps practices used in this project include:

* Git version control
* GitHub repository management
* GitHub Actions
* CI/CD pipelines
* Automated testing
* Automated builds
* Docker
* Docker Compose
* Environment configuration
* Build validation
* Deployment artifacts
* GitHub Secrets
* Production build automation

### Complete Technology Stack

**Frontend:**
React.js • JavaScript • HTML5 • CSS3 • Vite • Responsive Web Design

**Backend:**
Python • Flask • REST API • Backend Validation • Business Logic

**Database:**
SQLite • Relational Data Management • CRUD Operations

**Authentication:**
JWT Authentication • Password Hashing • Protected Routes

**API Integration:**
OpenStreetMap • Overpass API • Location-Based Services • External APIs

**DevOps:**
Docker • Docker Compose • GitHub Actions • CI/CD • Automated Testing • Build Automation • Deployment Pipeline

**Development Tools:**
Git • GitHub • npm • pip • Virtual Environment • Environment Variables

### Full Architecture

User
↓
React.js Frontend
↓
REST API
↓
Python Flask Backend
↓
Recommendation / Business Logic
↓
SQLite Database
↓
External APIs
↓
Docker Containers
↓
GitHub
↓
GitHub Actions
↓
CI/CD Pipeline
↓
Deployment

This makes NestWise Pakistan a **complete full-stack and DevOps-enabled web application**, rather than only a React frontend project.
