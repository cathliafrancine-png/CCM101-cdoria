# Mission 6: The Cloud Deployment Engineer

**Course:** CCM101 – Cloud Computing  
**Laboratory Activity:** Midterm Laboratory Exam – Mission 6  
**Project:** Nextcloud and MariaDB Multi-Container Deployment  
**Platform:** KillerCoda Ubuntu 24.04 Playground

---

## 1. Mission Overview

This laboratory activity focused on deploying a two-tier private cloud storage application using Docker Compose. The goal was to understand how multiple containers can work together to provide an application and its database.

In this project, Nextcloud served as the web application, while MariaDB handled the database. Both services were defined in a `docker-compose.yml` file and deployed together using a single Docker Compose command.

The activity also introduced Infrastructure as Code (IaC), where infrastructure configurations are written in files instead of relying only on manually entered commands.

## 2. Objectives

The objectives of this laboratory activity were to:

- Understand the concept of multi-tier application architecture.
- Identify the roles of the web/application tier and database tier.
- Create a Docker Compose YAML configuration using the Linux nano editor.
- Deploy Nextcloud and MariaDB as separate containers.
- Verify the running containers using Docker Compose commands.
- Access the Nextcloud installation interface through port 8080.
- Stop and remove the deployed containers properly.
- Document the deployment process using Markdown.
- Organize and maintain the laboratory output in a GitHub Cloud Computing Portfolio.

## 3. Commands Executed

The following commands were used during the laboratory activity.

| Command | Description |
|---|---|
| `mkdir nextcloud-deployment` | Created the deployment project directory. |
| `cd nextcloud-deployment` | Opened the project directory. |
| `pwd` | Displayed the current working directory. |
| `nano docker-compose.yml` | Created and edited the YAML configuration file. |
| `cat docker-compose.yml` | Displayed the contents of the Compose file. |
| `docker compose config` | Initially attempted configuration validation, but the Compose V2 command was unavailable. |
| `docker-compose --version` | Confirmed that Docker Compose V1.29.2 was installed. |
| `docker-compose config` | Successfully validated the YAML configuration. |
| `docker-compose up -d` | Created and started the Nextcloud and MariaDB containers. |
| `docker-compose ps` | Verified that both containers were running. |
| `cd /root/nextcloud-deployment` | Returned to the correct project directory before teardown. |
| `docker-compose down` | Stopped and removed the containers and their Compose network. |

### Deployment Verification

The `docker-compose ps` command confirmed that the Nextcloud and MariaDB containers were running successfully.

The Nextcloud installation interface was accessed through port `8080` using the KillerCoda browser environment. The administration account setup page appeared, confirming that the application was accessible.

The installation was intentionally left incomplete, following the laboratory instructions. The containers were then successfully stopped and removed using `docker-compose down`.

## 4. Skills Learned

Through this laboratory activity, I practiced several important cloud computing skills:

- **Multi-Tier Architecture:** Understanding how the application tier and database tier work together.
- **Docker Compose:** Managing multiple containers through one YAML configuration file.
- **Linux Commands:** Creating directories, navigating folders, and editing files using a terminal.
- **YAML Configuration:** Using proper indentation and environment variables to define services.
- **Container Networking:** Understanding how Nextcloud communicates with MariaDB using the database service name.
- **Port Mapping:** Accessing a web application running inside a container through a host port.
- **Infrastructure as Code:** Defining infrastructure settings in a reusable configuration file.
- **Technical Documentation:** Recording commands, deployment results, and screenshots using Markdown.
- **GitHub Portfolio Management:** Organizing and committing laboratory work in a structured repository.

## Deployment Evidence

### Docker Compose Deployment

![Successful Docker Compose Deployment](screenshots/compose-deployment.png)

### Nextcloud Installation Page

![Nextcloud Web Installation](screenshots/nextcloud-web.png)

### Docker Compose Teardown

![Successful Docker Compose Teardown](screenshots/compose-teardown.png)

---

## Conclusion

This mission helped me understand how Docker Compose simplifies the process of deploying applications that require multiple containers. By separating Nextcloud and MariaDB, I learned how the application and database can communicate while maintaining their own responsibilities.

The activity also demonstrated how Infrastructure as Code makes cloud deployment more organized and easier to repeat. Using Docker Compose, I was able to configure, deploy, verify, access, and shut down a two-tier application through a small set of terminal commands.
