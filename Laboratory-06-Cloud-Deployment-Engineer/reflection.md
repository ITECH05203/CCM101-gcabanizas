# Mission 6 Reflection

## 1. How does writing a `docker-compose.yml` file make a cloud engineer's job easier?

Creating a `docker-compose.yml` file makes deployment more organized because the settings for the application can be written in one place. Instead of remembering and entering several Docker commands, the engineer can use the same configuration whenever the application needs to be deployed again. This also makes the setup easier for another engineer to understand.

## 2. What happens if you make an indentation error in a YAML file?

YAML depends on proper spacing and indentation to understand the structure of the configuration. If I accidentally use a Tab or place a line at the wrong indentation level, Docker Compose may report an error and fail to read the file correctly. This showed me that even small formatting mistakes can prevent a deployment from working.

## 3. Why did we use environment variables like `MYSQL_PASSWORD`?

Environment variables allow important configuration values to be passed to the containers without placing them directly inside application commands. In this activity, they were used for database information such as the password, database name, and username. They also helped Nextcloud know which database settings it should use.

## 4. How did it feel to deploy Nextcloud in just a few minutes?

I found the deployment interesting because a complete web application and database could be started using one Compose command. Seeing the Nextcloud setup page in the browser made the process feel more practical than simply studying Docker commands.

## 5. How has my understanding of Cloud Computing evolved since Mission 1?

Since Mission 1, I have learned that cloud computing involves more than accessing online services. I have worked with Linux, cloud platforms, containers, storage, and now multi-container deployment. Mission 6 helped me understand how automation and Infrastructure as Code can make cloud environments easier to reproduce and manage.

