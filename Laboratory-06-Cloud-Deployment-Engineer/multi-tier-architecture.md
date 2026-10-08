# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is a system that separates an application into two main parts: the web/application tier and the database tier. These tiers work together to provide the application's features and manage its data. In this project, Nextcloud serves as the web application, while MariaDB manages the database.

## The Web/Application Tier

The web/application tier is responsible for handling user requests and providing the interface that users interact with. In our cloud deployment, Nextcloud allows users to access a private cloud storage system through a web browser. It processes HTTP requests and communicates with the database whenever information needs to be stored or retrieved.

## The Database Tier

The database tier is responsible for storing and managing the application's persistent information. In this project, MariaDB stores important Nextcloud data, such as user account information, application settings, and file metadata. It allows Nextcloud to retrieve and update these records when needed.

## Why Separate Them?

Separating the web application and database into different containers makes the system easier to organize, manage, and maintain. It also allows each container to be updated or restarted independently, which can make troubleshooting easier and reduce unnecessary changes to other parts of the application.
