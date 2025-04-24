Online Photographer Booking Website
Overview
The Online Photographer Booking Website is a user-friendly platform designed to connect clients with professional photographers for various occasions, such as weddings, events, portraits, and corporate shoots. Built as a mini-project by students at De Paul Institute of Science and Technology, this web application streamlines the process of discovering, booking, and managing photography services. Clients can browse photographer profiles, view portfolios, check real-time availability, and make secure payments, while photographers can manage bookings and showcase their work through a comprehensive dashboard.

Features

Client Features:
Search and filter photographers by style, location, and budget.
View detailed photographer profiles with portfolios, reviews, and pricing.
Real-time availability checking and booking.
Secure online payment integration.
Review and rating system for transparency.


Photographer Features:
Customizable profiles to showcase portfolios and expertise.
Dashboard to manage bookings, availability, and client communications.
Real-time updates for scheduling and notifications.


General Features:
Responsive design for seamless access on mobile and desktop devices.
Intuitive interface for easy navigation.
Scalable architecture to support future enhancements.



Technologies Used

Frontend: HTML, CSS, JavaScript, PHP
Backend: Python (Django), MySQL
Database: SQLite (development), MySQL (production)
Development Tools: Visual Studio Code, PyCharm
Browsers Supported: Google Chrome, Firefox, Internet Explorer
Other: Django ORM for database management, CSS preprocessors (e.g., Sass/LESS considerations)

Installation
To set up the project locally, follow these steps:
Prerequisites

Hardware:
Processor: Dual-core Intel or AMD
RAM: 2GB minimum
Disk Space: 250GB or more


Software:
Operating System: Windows 8/10
Python 3.x
MySQL Server
PHP (for frontend components)
Visual Studio Code or PyCharm
Git



Steps

Clone the Repository:
git clone https://github.com/your-username/online-photographer-booking-website.git
cd online-photographer-booking-website


Set Up Virtual Environment (for Python/Django):
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate


Install Dependencies:
pip install -r requirements.txt


Configure Database:

Set up MySQL and create a database named photographer_booking.
Update the database settings in settings.py:DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'photographer_booking',
        'USER': 'your_mysql_user',
        'PASSWORD': 'your_mysql_password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}




Run Migrations:
python manage.py makemigrations
python manage.py migrate


Set Up PHP Environment (if required for frontend):

Install XAMPP or a similar PHP server.
Place PHP files in the appropriate server directory (e.g., htdocs for XAMPP).


Start the Development Server:
python manage.py runserver


Access the application at http://localhost:8000.



Usage

For Clients:
Browse photographers by applying filters (style, location, budget).
View profiles, check availability, and book a session.
Complete payment securely and leave reviews post-session.


For Photographers:
Log in to the dashboard to set up your profile and portfolio.
Manage bookings, update availability, and communicate with clients.


For Admins:
Access the admin panel (/admin) to manage users, bookings, and platform settings.



Project Structure
online-photographer-booking-website/
├── manage.py               # Django project entry point
├── requirements.txt        # Python dependencies
├── photographer_app/       # Main Django app
│   ├── migrations/         # Database migrations
│   ├── templates/         # HTML templates
│   ├── static/            # CSS, JS, and images
│   ├── models.py          # Database models
│   ├── views.py           # Request handlers
│   └── urls.py            # URL routing
├── settings.py            # Django configuration
└── README.md              # Project documentation

Testing
The project includes the following testing levels:

Unit Testing: Tests individual modules (e.g., user authentication, booking logic).
Integration Testing: Verifies interactions between components (e.g., booking and payment systems).
System Testing: Ensures end-to-end functionality (e.g., booking workflow).
Security Testing: Protects against unauthorized access and data breaches.
Performance Testing: Evaluates responsiveness and scalability.

Limitations

Limited to predefined photography categories (e.g., weddings, events).
No built-in feedback system for individual bookings.
Basic fraud detection for payments (to be enhanced).

Future Enhancements

Implement a chatbot for user queries and support.
Add a quick-call feature for urgent bookings.
Enhance fraud detection with machine learning algorithms.
Expand support for additional photography niches.

Contributors

Maria Grazia Palatty
Ajal P P
Akshay Paul

License

This project is licensed under the MIT License. See the LICENSE file for details.

References

W3Schools
Python Official Site
Django Documentation
Bhatla T.P. et al., Understanding Credit Card Frauds, Cards Business Review, 2003.

