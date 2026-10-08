# Mission 6 Reflection

Completing Mission 6 helped me understand how Docker Compose makes cloud deployment easier and more organized. Instead of typing separate commands to create and connect different containers, I learned that a `docker-compose.yml` file can define everything in one place. With a single command, I was able to start both Nextcloud and MariaDB, which saved time and made the deployment process easier to manage.

One important lesson I learned was the importance of proper indentation in YAML files. Even a small mistake, such as using a Tab instead of spaces, can cause a parsing error or prevent Docker Compose from reading the configuration correctly. This taught me to be more careful when writing configuration files and to validate them before running any deployment.

I also understood why environment variables are useful. Variables such as `MYSQL_PASSWORD`, `MYSQL_USER`, and `MYSQL_DATABASE` allow us to provide important configuration values to the containers. However, I learned that passwords should be protected instead of being exposed in configuration files used for real deployments.

The most exciting part was seeing the Nextcloud installation page open in my browser after deploying the containers. At first, I thought setting up a cloud storage application would require many complicated steps. Seeing both containers running successfully made me feel more confident. I also encountered a problem when shutting down the containers because I was in the wrong directory, but I learned how to identify and correct it.

Since our earlier cloud computing activities, my understanding has developed from learning basic cloud concepts to working with actual tools and environments. I now understand that cloud computing also involves configuring services, connecting applications, managing containers, and documenting the process. Overall, this mission helped me become more careful, confident, and responsible when working with cloud technologies.
