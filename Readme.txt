Docker Compose Setup for Ecommerce Application

This Docker Compose configuration sets up an environment for an Ecommerce application, including a MySQL database, backend, and UI components.

Follow these steps to use the Docker Compose configuration:

1. Prerequisites:
   - Install Docker: Make sure you have Docker installed on your system. You can download it from https://www.docker.com/get-started

2. Initializing some starting data in the database:
   - 'Database.sql' used to initialize the database, needs to be in the same directory as the 'docker-compose.yml' file.

3. Run the Containers:
   - Open a terminal or command prompt.
   - Navigate to the directory containing the 'docker-compose.yml' and 'Database.sql' files.
   - Run the following command:
     ```
     docker-compose up -d
     ```
   - Docker Compose will start the defined services in the background.

4. Access the Application (Please wait for couple of minutes in order for the database and back-end to finish initialization):
   - Open your browser and go to http://localhost:8080
   - Use username: admin password: admin@pass to login into the application as admin and explore its capabilities.
   - Sign up to check the application from a Customer point of view

5. Shut Down the Containers:
   - To stop the containers, run the following command:
     ```
     docker-compose down
     ```
   - This will stop and remove the containers, but data stored within the database container might be lost. If you want to persist data between container restarts, consider using Docker volumes.
