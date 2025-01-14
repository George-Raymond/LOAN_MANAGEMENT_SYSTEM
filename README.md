# LOAN_MANAGEMENT_SYSTEM
FRONT_END
# Precious Investment Co. Ltd - Loan Management System

## Overview
This project is a web-based loan management system for **Precious Investment Co. Ltd**, a financial institution providing loan services to individuals, businesses, and communities. The system allows users to apply for loans, manage loan-related information, and interact with the company through a user-friendly interface. The application is built using HTML, CSS, and JavaScript, with a focus on simplicity, security, and transparency.

---

## Features
1. **User Authentication**:
   - Login and registration system for users.
   - Secure password handling and token-based authentication.

2. **Loan Application**:
   - Multi-step loan application process:
     - **Mkopaji (Borrower)**: Collects borrower's personal and financial details.
     - **Mdhamini (Guarantor)**: Collects guarantor's information.
     - **Ofisi (Office)**: Internal use for loan approval and recommendations.
   - File upload for borrower and guarantor photos.
   - Dynamic form validation and data storage using `localStorage`.

3. **Navigation**:
   - Responsive navigation bar with active link highlighting.
   - Easy access to different sections: Borrower, Guarantor, Office, About Us, Register, and Login.

4. **About Us Page**:
   - Detailed information about the company, including mission, vision, values, and contact details.

5. **Responsive Design**:
   - Mobile-friendly layout with a clean and modern design.
   - Gradient backgrounds and consistent styling across all pages.

6. **Data Storage**:
   - Temporary storage of form data using `localStorage`.
   - Combined data submission for loan applications.

7. **API Integration**:
   - Integration with a backend API for user registration, login, and loan submission.

---

## Pages
1. **Home (About Us)**:
   - Provides an overview of the company, including its mission, vision, values, and contact information.

2. **Mkopaji (Borrower)**:
   - Form for collecting borrower's personal, residential, and employment details.

3. **Mdhamini (Guarantor)**:
   - Form for collecting guarantor's personal and employment details.

4. **Ofisi (Office)**:
   - Internal form for loan approval and recommendations by loan officers and branch managers.

5. **Register**:
   - User registration form with username and password fields.

6. **Login**:
   - User login form with token-based authentication.

---

## Technologies Used
- **Frontend**:
  - HTML5
  - CSS3 (with gradients, flexbox, and responsive design)
  - JavaScript (for form handling, data storage, and API integration)

- **Backend**:
  - API endpoints for user authentication and loan submission (e.g., `https://loan-management-system-jf05.onrender.com`).

- **Tools**:
  - `localStorage` for temporary data storage.
  - Fetch API for backend communication.

---

## How to Use
1. **Register**:
   - Navigate to the **Register** page and create an account by providing a username and password.

2. **Login**:
   - Use your credentials to log in on the **Login** page.

3. **Apply for a Loan**:
   - Start the loan application process by filling out the **Mkopaji** form.
   - Proceed to the **Mdhamini** form to provide guarantor details.
   - Complete the process on the **Ofisi** page for internal approval.

4. **View Company Information**:
   - Visit the **About Us** page to learn more about Precious Investment Co. Ltd.

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/loan-management-system.git
   ```
2. Open the project folder:
   ```bash
   cd loan-management-system
   ```
3. Open the `index.html` file in your browser to view the application.

---

## API Endpoints
- **Login**: `POST https://loan-management-system-jf05.onrender.com/token`
- **Register**: `POST https://loan-management-system-jf05.onrender.com/register`
- **Loan Submission**: `POST https://your-api-endpoint.com/submit`

---

## Styling
- **Colors**:
  - Primary: Green (`#4CAF50`)
  - Secondary: Light Green (`#81C784`)
  - Background: Gradient from white to light green.

- **Fonts**:
  - Arial, sans-serif.

- **Responsive Design**:
  - Flexbox for layout.
  - Media queries for mobile compatibility.

---

## Future Improvements
1. **Backend Integration**:
   - Connect the frontend to a fully functional backend for persistent data storage.
2. **User Dashboard**:
   - Add a dashboard for users to track loan status and payments.
3. **Admin Panel**:
   - Create an admin panel for managing loans, users, and approvals.
4. **Enhanced Security**:
   - Implement stronger authentication mechanisms (e.g., OAuth, JWT).

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contact Information
- **Company Name**: Precious Investment Co. Ltd
- **Address**: P.O. Box 616, Morogoro – Ifakara Branch
- **Phone**: 0746-667797
- **Email**: info@preciousinvestment.co.tz

---

**© 2025 Precious Investment Co. Ltd. All Rights Reserved.**
