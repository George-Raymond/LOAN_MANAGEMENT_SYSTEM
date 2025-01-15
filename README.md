Precious Investment Co. Ltd - Loan Management System
This project is a Loan Management System developed for Precious Investment Co. Ltd. It allows users to apply for loans, manage loan applications, and handle administrative tasks such as approvals and tracking. The system is built using PHP for the backend, HTML/CSS for the frontend, and MySQL for database management.

✨ Features
User Authentication:

Users can register and log in to access the system.

Session management ensures secure access to authenticated pages.

Loan Application:

Borrowers can fill out loan application forms with personal details, employment information, and collateral details.

Guarantors can provide their details as part of the loan application process.

Office Use:

Loan officers can review and recommend loan applications.

Supervisors and branch managers can approve or reject loan applications.

Data Persistence:

All form data is stored in a MySQL database for future reference and processing.

Security:

CSRF protection to prevent cross-site request forgery attacks.

Password hashing for secure storage of user credentials.

Responsive Design:

The system is mobile-friendly and works seamlessly across devices.

📂 Project Structure
The project consists of the following files:

File Name	Description
mkopaji.php	Loan application form for borrowers.
mdhamini.php	Form for guarantors to provide their details.
ofisi.php	Administrative interface for loan officers, supervisors, and branch managers.
register.php	User registration page.
login.php	User login page.
dashboard.php	Dashboard for authenticated users (not implemented in the provided code).
logout.php	Logs out the user and destroys the session.
styles.css	Contains the styling for the project.
🛠️ Setup Instructions
Prerequisites
Web Server: Apache or Nginx.

PHP: Version 7.0 or higher.

MySQL: For database management.

Browser: Chrome, Firefox, or any modern browser.

Steps
Clone the Repository:

bash
Copy
git clone https://github.com/George-Raymond/precious-investment.git
cd precious-investment
Set Up the Database:

Create a MySQL database named precious_investment.

Import the following SQL schema:

sql
Copy
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50) NOT NULL UNIQUE,
    password VARCHAR(255) NOT NULL
);

CREATE TABLE loan_applications (
    id INT AUTO_INCREMENT PRIMARY KEY,
    fullName VARCHAR(100) NOT NULL,
    phone VARCHAR(15) NOT NULL,
    photoPath VARCHAR(255),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

CREATE TABLE ofisi_data (
    id INT AUTO_INCREMENT PRIMARY KEY,
    loanRecommendation TEXT NOT NULL,
    reason TEXT NOT NULL,
    loanOfficerName VARCHAR(100) NOT NULL,
    loanOfficerSignature VARCHAR(100) NOT NULL,
    loanOfficerDate DATE NOT NULL,
    supervisorName VARCHAR(100) NOT NULL,
    supervisorSignature VARCHAR(100) NOT NULL,
    supervisorDate DATE NOT NULL,
    branchManagerName VARCHAR(100) NOT NULL,
    branchManagerSignature VARCHAR(100) NOT NULL,
    branchManagerDate DATE NOT NULL
);
Configure Database Connection:

Update the database credentials in each PHP file (e.g., register.php, mkopaji.php):

php
Copy
$servername = "localhost";
$username_db = "root";
$password_db = "";
$dbname = "precious_investment";
Run the Application:

Place the project files in your web server's root directory (e.g., htdocs for XAMPP or www for WAMP).

Access the application via your browser:

Copy
http://localhost/precious-investment
🚀 Usage
Registration:

Navigate to register.php to create a new account.

Fill in the required details (username and password).

Login:

Navigate to login.php to log in with your credentials.

Loan Application:

After logging in, go to mkopaji.php to fill out the loan application form.

Provide all required details, including personal information, employment details, and collateral.

Guarantor Details:

Navigate to mdhamini.php to provide guarantor details.

Office Use:

Loan officers, supervisors, and branch managers can use ofisi.php to review and approve loan applications.

Logout:

Click the "Logout" link to securely log out of the system.

🔒 Security Considerations
CSRF Protection:

Each form includes a CSRF token to prevent cross-site request forgery attacks.

Password Hashing:

User passwords are hashed using PHP's password_hash() function for secure storage.

Session Management:

Session IDs are regenerated periodically to prevent session fixation attacks.

Input Validation:

Both client-side (JavaScript) and server-side (PHP) validation are implemented to ensure data integrity.

🤝 Contributing
Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

Fork the repository.

Create a new branch for your feature or bugfix.

Commit your changes.

Submit a pull request.

📜 License
This project is licensed under the MIT License. See the LICENSE file for details.

📞 Contact
For any questions or feedback, please contact:

Name: George Raymond

Email: raysgeorge429@gmail.com

GitHub: George-Raymond
