# Mission Reflection

This activity helped me understand why containers are useful in cloud computing and how they are different from Virtual Machines. For a Docker container, the setup is much faster because there is no need to install and boot a separate operating system. In our activity, we were able to pull the Nginx image and run the container within a short time. Compared with installing an operating system on a VM, Docker makes application deployment more lightweight and faster.

The port mapping `-p 8080:80` is necessary because the web server is running inside the container on port 80, while we access it through port 8080 on the host. Without this mapping, the Nginx service inside the container would not be directly accessible through the host port we used. By mapping the ports, we were able to send a request using `curl http://localhost:8080` and see the Nginx welcome page.

When `docker rm` is used, the specified stopped container is removed. This means the container itself and its writable data are deleted. The Docker image is not removed by `docker rm`, so the image can still be used to create another container later.

I also learned that containerization can improve collaboration between developers and IT operations teams because applications can be packaged with their required environment and deployed in a more consistent way. Developers and operations teams can work with the same container setup, which can make testing and deployment easier.

My GitHub portfolio is also evolving because I am now adding organized laboratory activities with documentation, commands, screenshots, and reflections. Instead of only keeping the outputs of activities, I am building a record of what I learned and the technical tasks I completed. This makes my portfolio more organized and shows my progress in cloud computing.
