# Angel Life Pharmacy Website

The Angel Life Pharmacy is an online order placing system designed for customers and staff to track and manage orders efficiently and effectively. This web portal dynamically renders the page according to the logged-in user's state and is optimized for all devices, including mobile. The application is aimed at modernizing the traditional pharmacy experience by allowing customers to purchase drugs online with a valid prescription, thus reducing the need to physically visit the pharmacy. This system facilitates different user roles such as admin, staff, and customer, each with specific functionalities to streamline pharmacy operations.


## Table of Contents

1. [Installation](#installation)
2. [Technologies Used](#technologies-used)
3. [Devops](#devops)
4. [Features](#features)
5. [Contributing](#contributing)


## Installation

### Front Setup

- Clone the repository to a designated location on your device.
- Navigate to frontend directory.
- Run npm i to install required dependancies
- Start the frontend development server using npm start.

### Backend Setup

- Clone the repository to a designated location on your device.
- Navigate to backend directory.
- Run npm i to install required dependancies
- Create the .env file and check the config.js file to setup the .env file with the required enviromental variables.
- Start the backend development server using npm start.

## Technologies Used

#### Languages

- Html/Css - (Used for user interface development)
- Typescript - (Used for application logic)

#### Frameworks

- Frontend - Angular
- Backend - Node.js with Express.js

#### Third Party API and Utils

- Multer - (Middleware for handling multipart/form-data)
- AWS SDK - (Interact with AWS S3 bucket)
- bcrypt - (Password hashing)
- @hapi/joi - (Data validation)
- Socket.io - (Real-time bidirectional event-based communication)
- Chai - (Assertion library for testing)
- Chai-HTTP - (HTTP integration testing with Chai)
- Mocha- - (JavaScript test framework)

#### Database

- MongoDB Atlas - (Used for storing and managing application data)

## Devops

### CI/CD Pipeline

The CI/CD pipeline is managed via GitHub workflows, integrated with Netlify for the frontend and Render for the backend. The workflow includes the following steps:

- Frontend - Runs npm install and build on each commit and deploys to Netlify via a webhook trigger.
- Backend - Runs npm install and tests on each commit and if tests pass, deploys to Render via a webhook trigger.

Deployments can be managed and blocked through respective dashboards if needed.


## Features

### General Features

- Secure login for admin, staff, and customers.
- Dynamic home page accessible to all users.
- View and update profile details.
- Password management to update passwords securely.
- Order management to view order details.
- Live chat facility for real-time communication between users and staff.

### Admin Features

- Add and manage employees.
- Access all staff functionalities.

### Staff Features

- Accept and update order statuses.
- Edit order details and add new items to orders.
- Perform CRUD operations on customer details.
- Reject incomplete orders.
- View all orders.

### Customer Features

- Place new orders.
- Register via a registration form.
- View and manage personal orders.
- Cancel pending orders.


## Contributing

- Fork the project.
- Create your feature branch (git checkout -b feature/your-feature).
- Commit your changes (git commit -am 'Add some feature').
- Push to the branch (git push origin feature/your-feature).
- Create a new Pull Request.
