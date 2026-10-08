# online-voting-system
# Online Voting System

A secure, intuitive, and responsive **PHP-based Online Voting System** designed to digitize election processes. This web application allows administrators to manage elections, candidates, and voter registrations, while enabling registered voters to cast their ballots securely online.

## 🚀 Features

### Admin Dashboard
* **Voter Management:** Approve, reject, or delete voter registrations.
* **Candidate Management:** Add, edit, or remove candidates with their respective parties/positions.
* **Election Controls:** Start, pause, or finalize election timelines.
* **Real-Time Analytics:** View live voting statistics and graphical result representations.

### Voter Portal
* **Secure Authentication:** Multi-factor or secure password-based login.
* **Dynamic Ballot Paper:** View active elections, positions, and competing candidates.
* **One-Vote Restriction:** Smart restriction algorithms preventing duplicate voting.
* **Receipt Generation:** Instant voting confirmation after casting a ballot.

## 🛠️ Tech Stack

* **Backend:** PHP (8.x recommended)
* **Database:** MySQL / MariaDB
* **Frontend:** HTML5, CSS3, Bootstrap 5, JavaScript (jQuery)
* **Server Compatibility:** Apache / XAMPP / WAMP / MAMP

## 📋 Prerequisites

Before setting up the project, ensure you have the following installed:
* PHP >= 8.0
* MySQL Server
* A local web server environment (e.g., **XAMPP**)

## 🔧 Installation & Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com
   cd online-voting-system
   ```

2. **Database Configuration:**
   * Open your browser and navigate to `http://localhost/phpmyadmin/`.
   * Create a new database named `voting_system`.
   * Import the provided SQL file (`database/voting_system.sql`) into your newly created database.

3. **Establish Connection:**
   * Open the database configuration file (typically `config/db.php` or `includes/connection.php`).
   * Update your database credentials if they differ from the default setup:
     ```php
     define('DB_SERVER', 'localhost');
     define('DB_USERNAME', 'root');
     define('DB_PASSWORD', '');
     define('DB_NAME', 'voting_system');
     ```

4. **Run the Application:**
   * Move the project folder into your local server's root directory (e.g., `C:/xampp/htdocs/`).
   * Access the voter application via `http://localhost/online-voting-system/`.
   * Access the admin area via `http://localhost/online-voting-system/admin/`.

## 🔒 Security Implementations

* **Password Hashing:** Implemented using PHP's native `password_hash()` function.
* **SQL Injection Prevention:** Structured queries utilizing PDO or prepared MySQLi statements.
* **Session Validation:** Strict session tokens to prevent unauthorized dashboard access.
* **Data Sanitization:** Robust input filtering protecting against Cross-Site Scripting (XSS).

## 🤝 Contributing

Contributions make the open-source community an amazing place to learn, inspire, and create.
1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
