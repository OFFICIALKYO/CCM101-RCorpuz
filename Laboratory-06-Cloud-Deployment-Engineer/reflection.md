# Mission 6 Reflection

Writing a `docker-compose.yml` file helped me understand how to manage multiple containers in a simple way. Instead of typing many `docker run` commands, I can just put all the configurations in one YAML file. Using `docker-compose up -d`, I can start the application and database together. It saves time and makes the deployment easier, especially when working with more than one container.

One thing I learned is that YAML indentation is very important. If I use incorrect spaces or tabs, the configuration might show an error and the containers will not start properly. During this activity, I realized that even a small mistake in the code can affect the whole deployment. Because of this, I learned to check my YAML file carefully before running it.

Environment variables are also important because they allow us to configure the database connection, username, and password without changing the application image. For example, `MYSQL_PASSWORD` is used to set the database password. I learned that these variables make the configuration easier to manage, although sensitive passwords should be protected and not shared publicly.

Deploying Nextcloud was one of the interesting parts of this mission. At first, I thought setting up a cloud storage system would be difficult because it needs an application and a database. But after using Docker Compose, I was surprised that I could run the services using only a few commands. Seeing the Nextcloud login page made me happy because I was able to experience how cloud storage works.

Since Mission 1, my understanding of cloud computing has improved. Before, I only knew that cloud computing was used for storing files and accessing services through the internet. Now, I understand that it also involves containers, networking, databases, and automation. This mission taught me that being a cloud engineer requires patience, problem-solving skills, and understanding how different services work together. I know I still have many things to learn, but this activity helped me gain more confidence in using Docker and Docker Compose.
