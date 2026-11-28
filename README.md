# TrackShield

TrackShield is a PHP and MySQL web application for reporting, tracking, and managing railway emergencies. Passengers can report incidents, administrators can verify and assign them, and response teams can manage incidents through resolution.

## Technology

- PHP 8.0+ with PDO
- MySQL 5.7+ or MariaDB 10.3+
- HTML, CSS, and vanilla JavaScript
- Chart.js 4.4.1 (bundled locally)

## Features

- Role-based authentication for passengers, administrators, and response teams
- Emergency reporting, assignment, status tracking, and notifications
- Admin dashboards, team and user management, and analytics
- Input validation, CSRF protection, session hardening, and secure file uploads

## Project files

The application source is in [`TrackShield-main/`](./TrackShield-main/). Its detailed feature list, folder structure, security notes, and production checklist are in the [application README](./TrackShield-main/README.md).

## Local setup (XAMPP)

1. Copy the contents of `TrackShield-main/` into `C:\xampp\htdocs\TrackShield\`.
2. Start Apache and MySQL from the XAMPP Control Panel.
3. Import `database/trackshield_db.sql` into phpMyAdmin.
4. Configure database access in `config/database.php`, or set `TS_DB_HOST`, `TS_DB_PORT`, `TS_DB_NAME`, `TS_DB_USER`, and `TS_DB_PASS`.
5. Open [http://localhost/TrackShield/](http://localhost/TrackShield/).

The SQL file seeds demo accounts. Change or remove their passwords before deploying the application.
