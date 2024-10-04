# E-Voting System

This repository contains the source code for an **E-Voting System** that allows users to cast votes online securely and efficiently. The system leverages modern web technologies and ensures a smooth, user-friendly voting experience while maintaining the confidentiality and integrity of each vote.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Overview

The **E-Voting System** is designed to provide a seamless and secure online voting experience. It ensures voter authentication and vote integrity while allowing users to vote from the comfort of their homes. This project demonstrates how a digital voting system can be implemented for various use cases, including elections, polls, and other voting events.

## Features
- **User Authentication**: Secure login for voters to ensure the right people are voting.
- **Admin Dashboard**: Provides an interface for administrators to manage candidates and monitor the voting process.
- **Vote Casting**: Allows users to cast their votes securely.
- **Real-time Vote Counting**: Dynamic vote count updates as votes are cast.
- **Secure and Encrypted**: Votes are encrypted to prevent tampering and ensure confidentiality.
- **Responsive Design**: Optimized for both desktop and mobile devices.

## Technologies Used

**Frontend**:
- HTML5, CSS3, JavaScript

**Backend**:
- Node.js, Express.js

**Database**:
- MongoDB

**Authentication**:
- JWT (JSON Web Tokens)

**Other Tools**:
- bcrypt for password hashing
- Mongoose for database interaction

## Setup Instructions

### Prerequisites

Ensure you have the following installed on your local machine:
- Node.js (v14 or above)
- MongoDB (ensure it is running locally or use a cloud MongoDB service like MongoDB Atlas)

### Steps to Set Up Locally

1. **Clone the repository**:
    ```bash
    git clone https://github.com/mohammedbilal09/E-Voting-system.git
    ```

2. **Navigate to the project directory**:
    ```bash
    cd E-Voting-system
    ```

3. **Install dependencies**:
    ```bash
    npm install
    ```

4. **Set up environment variables**:
   - Create a `.env` file in the root of the project.
   - Add the following variables:
     ```bash
     PORT=3000
     MONGO_URI=<Your MongoDB connection string>
     JWT_SECRET=<Your secret key for JWT>
     ```

5. **Start the application**:
    ```bash
    npm start
    ```

6. **Access the app**: 
   Open a browser and go to `http://localhost:3000`

## Usage

Once the application is up and running:

- **For Voters**: 
  - Register or log in to cast your vote.
  - Once authenticated, you can view the list of candidates and cast your vote.
  
- **For Admins**: 
  - Admins can log in with the admin credentials.
  - Manage candidates, monitor vote counts, and access administrative features from the dashboard.

## Contributing

Contributions are welcome! If you have any improvements or suggestions, feel free to open a pull request. Please ensure your code follows best practices and is well-documented.

### Steps for Contribution

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Submit a pull request for review.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
