# DashTally
A fancy mileage and income tracker for 1099 delivery


Delivery Miles Tracker

Delivery Miles Tracker is a web application designed for delivery drivers to track their shifts, mileage, pay earned, and platform usage. It offers a modern, responsive interface for managing and analyzing shift data, helping drivers optimize their routes, calculate reimbursements, and monitor earnings over time.
Features

    Shift Management: Start and end shifts with odometer readings, time tracking, and earnings.
    Mileage and Earnings Calculation: Automatically calculate total miles, total hours, pay per hour, and pay per mile for each shift.
    Platform Tracking: Select platforms used during a shift (e.g., DoorDash, Grubhub, UberEats).
    Statistics Dashboard: View aggregated statistics such as total hours, miles, pay, pay/hour, pay/mile, and IRS mileage reimbursement.
    Date Range Filtering: Filter ended shifts by a specific date range.
    Excel Import/Export: Import and export shift data using Excel files.
    User Authentication: Secure login for administrators with password hashing and change password functionality.
    Responsive Design: Mobile-optimized interface that uses numeric keyboards for appropriate fields.
    Theming: Dark mode support and professional design elements.

Setup and Installation
Prerequisites

    Python 3.7 or higher
    Flask and related dependencies (see requirements.txt)
    SQLite (for the default database)

Installation

    Clone the Repository:

git clone https://github.com/yourusername/delivery-miles-tracker.git
cd delivery-miles-tracker

Create a Virtual Environment and Install Dependencies:

    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    pip install -r requirements.txt

Database Initialization

Before running the application, initialize the database:

flask initdb

This command creates the database, tables, and a default admin user. You can modify the initdb command in app.py to suit your initialization needs.
Running in Development Mode

To run the application in development mode:

export FLASK_APP=app.py
export FLASK_ENV=development
flask run

The application will be available at http://127.0.0.1:5000 by default.
Production Setup

The default username is: admin
the password is: ChangeMe123

Usage

    Login: Access the login page, enter your admin credentials to log in.
    Start a Shift: Click "Start Shift," fill in your odometer reading, and begin tracking.
    End a Shift: Use the "View Timer" or "End Shift" button to finalize your shift, entering end time, ending odometer, pay earned, and selecting platforms.
    View Statistics: Filter and view past shifts, see aggregated statistics, and export/import data as needed.
    Options: Change password, adjust IRS mileage rate, import/export data, and toggle night mode via the options page.

Contributing

Contributions, suggestions, and improvements are welcome! Feel free to open issues or submit pull requests.
License

This project is licensed under the MIT License. See the LICENSE file for details.
