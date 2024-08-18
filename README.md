<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## Available API Routes

This section lists all the available routes for the `doc_app_Laravel` project, including API endpoints and authentication routes.

### Public Routes

- **Login**
  - `GET /login`: Display the login form.
  - `POST /login`: Handle login requests.

- **Register**
  - `GET /register`: Display the registration form.
  - `POST /register`: Handle registration requests.

- **Forgot Password**
  - `GET /forgot-password`: Display the form to request a password reset link.
  - `POST /forgot-password`: Handle requests to send the password reset link.
  - `GET /reset-password/{token}`: Display the password reset form.
  - `POST /reset-password`: Handle the password reset requests.

### User Routes

- **User Profile**
  - `GET /user/profile`: Display the user profile.
  - `PUT /user/profile-information`: Update the user profile information.
  - `PUT /user/password`: Update the user password.

- **Two-Factor Authentication**
  - `GET /user/two-factor-challenge`: Display the two-factor authentication challenge.
  - `POST /two-factor-challenge`: Handle two-factor authentication verification.
  - `POST /user/two-factor-authentication`: Enable two-factor authentication.
  - `DELETE /user/two-factor-authentication`: Disable two-factor authentication.
  - `GET /user/two-factor-qr-code`: Display the QR code for two-factor authentication setup.
  - `GET /user/two-factor-recovery-codes`: Display the recovery codes for two-factor authentication.
  - `POST /user/two-factor-recovery-codes`: Regenerate two-factor authentication recovery codes.
  - `GET /user/two-factor-secret-key`: Display the two-factor authentication secret key.

- **API Tokens**
  - `GET /user/api-tokens`: Display the user's API tokens.

- **Confirm Password**
  - `GET /user/confirm-password`: Display the confirm password form.
  - `POST /user/confirm-password`: Handle confirm password requests.
  - `GET /user/confirmed-password-status`: Check if the user's password is confirmed.

### Appointment Routes

- **Appointments**
  - `GET /api/appointments`: Retrieve a list of appointments.
  - `POST /api/book`: Book a new appointment.

### User Interaction Routes

- **Favorites**
  - `POST /api/fav`: Add a doctor to the user's favorites.

- **Reviews**
  - `POST /api/reviews`: Submit a review for a doctor.

### Authentication Routes

- **Login**
  - `POST /api/login`: Authenticate the user.

- **Logout**
  - `POST /api/logout`: Log out the authenticated user.

- **Register**
  - `POST /api/register`: Register a new user.

### System Routes

- **Dashboard**
  - `GET /dashboard`: Display the main dashboard.

### Ignition (Error Handling)

- `GET /_ignition/health-check`: Perform a health check.
- `POST /_ignition/execute-solution`: Execute a solution for an error.
- `POST /_ignition/update-config`: Update the Ignition configuration.

### Privacy & Terms

- **Privacy Policy**
  - `GET /privacy-policy`: Display the privacy policy.

- **Terms of Service**
  - `GET /terms-of-service`: Display the terms of service.
