# Car Zone

![License](https://img.shields.io/badge/license-MIT-blue.svg)

## Description

Car Zone is a web application developed using Django, HTML, CSS, JavaScript, and jQuery. It serves as an online car dealership where users can register, browse cars, and make purchases. The project also includes an admin panel for sellers to manage the inventory and other functionalities. Users can contact sellers through a messaging system, and these messages are sent to the seller's email.

## Features

- **User Registration**: Users can register and create an account.
- **Browse Cars**: Users can view a list of available cars.
- **Purchase Cars**: Users can purchase cars through the application.
- **Admin Panel**: Django admin panel for sellers to manage car listings and other aspects of the dealership.
- **Messaging System**: Users can send messages to sellers, which are delivered to the seller via email.

## Technologies

- **Python**: Programming language.
- **Django**: Web framework for building the application.
- **HTML/CSS**: For structuring and styling the frontend.
- **JavaScript**: For interactive elements and client-side functionality.
- **jQuery**: For simplifying DOM manipulation and event handling.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/mayis999/car-zone.git
    ```
2. **Set up a virtual environment** (recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```
3. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```
4. **Apply database migrations**:
    ```bash
    python manage.py migrate
    ```
5. **Create a superuser** (optional, for accessing the admin interface):
    ```bash
    python manage.py createsuperuser
    ```
6. **Configure email settings**:
    Update the `EMAIL_BACKEND` and related settings in your `settings.py` file to ensure that messages are sent correctly. For example:
    ```python
    EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
    EMAIL_HOST = 'smtp.example.com'
    EMAIL_PORT = 587
    EMAIL_USE_TLS = True
    EMAIL_HOST_USER = 'your-email@example.com'
    EMAIL_HOST_PASSWORD = 'your-email-password'
    ```
7. **Run the development server**:
    ```bash
    python manage.py runserver
    ```

## Usage

1. **Start the server** by running the `manage.py` script.
2. **Access the application** through your web browser at `http://localhost:8000` (or the URL provided by your application).
3. **Register and log in** to browse cars and make purchases.
4. **Sellers** can access the admin panel at `http://localhost:8000/admin/` to manage their inventory and other aspects of the dealership.
5. **Send messages** through the application, which will be sent to the seller's email.
