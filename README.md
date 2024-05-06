Installation Instructions:
1. Set up the Environment:
Download and install the XAMPP stack (or any LAMP/WAMP/MAMP stack). XAMPP includes an Apache server, MySQL database, and PHP for backend processing.
Ensure that the Apache and MySQL services are running in the XAMPP control panel.

2. Clone or Download the Project:
Access the GitHub repository or download the project archive provided.
Extract the project files into the `htdocs` folder within the XAMPP installation directory. This directory is the web server's root folder.

3. Database Setup:
Open the XAMPP control panel and start "phpMyAdmin" (or use any MySQL client).
Create a new database named `rentsys`.
Within the project files, locate the SQL script that defines the tables and initial data for the `rentsys` database.
Import the SQL script:
     1. In `phpMyAdmin`, select the `rentsys` database.
     2. Go to the "Import" tab.
     3. Click "Choose File" and select the SQL file from your project directory.
     4. Click "Go" to import the database structure and data.

4. Configure Database Connection:
In the project files, locate the database connection configuration file (usually `conn.php` or similar).
Ensure that the credentials match the local MySQL installation (default XAMPP credentials are usually `root` for the user and an empty password).
If necessary, adjust the database name to `rentsys`.

5. Adjust Application Configuration:
Verify the application configuration settings, such as URLs and paths, especially if the project files are not in the default location.

6. Test the Application:
Launch a web browser and navigate to `http://localhost/{project-folder}`.
Ensure all pages load correctly and that the registration/login functionality works.
Test the database connectivity by trying to create new tenant or landlord accounts.

7. Troubleshooting:
If there are issues with the application, refer to the error logs (`xampp\apache\logs\error.log`) for debugging.
Ensure that the database credentials and table structures are consistent.

8. Further Customization:
I could customize the project to fit your specific needs or enhance functionality by modifying the HTML, PHP, CSS, and JavaScript files.
