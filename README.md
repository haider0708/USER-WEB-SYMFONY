
# Health App Project

## Overview

This project is a web application built with Symfony 5, designed to provide secure access to a health page for users and an admin dashboard with advanced features.
The application supports encrypted user data, secure login, role-based access for users and admins, and additional features for SMS notifications, email notifications, and password reset functionality.

## Features

1. **User Login System**: Users can securely log in to access their personalized health page.
2. **Admin Dashboard**: Admins can log in to access a dashboard that provides an overview of key statistics, accessible only to users with the Admin role.
3. **Role-Based Security**: Separate roles for regular users and admins, with distinct permissions.
4. **Data Encryption**: User data is encrypted using the SHA-2 hashing algorithm to enhance data security.
5. **SMS and Email Notifications**: The application supports SMS and email notifications for critical actions, including login alerts and password resets.
6. **Password Reset Functionality**: Users can reset their password through an automated, secure process.
7. **Persistent Encrypted Data Storage**: Encrypted user data is securely stored and accessible for authorized use.

## Getting Started

### Prerequisites

- PHP >= 7.4
- Composer
- Symfony 5
- MySQL or PostgreSQL
- Node.js and npm (for frontend dependencies)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/haider0708/USER-WEB-SYMFONY.git
   ```

2. Install dependencies:
   ```bash
   composer install
   ```

3. Configure your database in the `.env` file:
   ```plaintext
   DATABASE_URL=mysql://username:password@127.0.0.1:3306/health_app
   ```

4. Run the migrations to set up the database schema:
   ```bash
   php bin/console doctrine:migrations:migrate
   ```

5. Install frontend dependencies:
   ```bash
   npm install
   npm run dev
   ```

### Usage

1. Start the Symfony server:
   ```bash
   symfony server:start
   ```

2. Access the application at `http://localhost:8000`.

3. Register a new user or log in with admin credentials to access the dashboard.

### Security & Encryption

- **User Data Encryption**: All user data is encrypted with SHA-2, ensuring that sensitive information remains secure.
- **Role Management**: Symfony's security features are utilized to restrict access to certain pages based on user roles.

### Additional Features

- **Notifications**: SMS and email notifications are triggered for key actions, such as logins and password resets.
- **Password Reset**: Users can request a password reset link via email to securely update their password.
- **Session Management**: User data is stored securely within the navigation bar and a variable, allowing authorized parts of the application to access it as needed.

## Built With

- Symfony 5 - PHP framework for web applications
- Doctrine ORM - For database interactions
- SHA-2 - For encryption of sensitive data
- Twig - For templating
- JavaScript and CSS - For frontend features

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.



