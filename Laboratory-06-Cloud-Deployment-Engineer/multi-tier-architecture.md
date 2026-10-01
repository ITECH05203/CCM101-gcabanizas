# Multi-Tier Architecture

## Two-Tier Architecture

A two-tier architecture is a system divided into two main parts that work together. One part handles the application and user interaction, while the other part manages the data needed by the application. In this activity, Nextcloud serves as the application and MariaDB acts as the database.

## The Web/Application Tier

The web/application tier is responsible for providing the application that users interact with through a web browser. It receives HTTP requests from users and processes the actions performed in the Nextcloud interface. In this setup, the Nextcloud container serves as the web/application tier.

## The Database Tier

The database tier handles the storage and management of information required by the application. MariaDB stores persistent information such as user details and other Nextcloud-related data. Keeping the database in its own container allows the application and its data management functions to remain separated.

## Why Separate Them?

Using separate containers makes the system easier to organize and manage because each container has a specific responsibility. The web application and database can also be maintained independently, which makes troubleshooting and future changes more manageable.

