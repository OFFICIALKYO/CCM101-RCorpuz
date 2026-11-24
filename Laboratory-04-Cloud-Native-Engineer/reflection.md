# Mission Reflection

Setting up a Docker container is much faster than installing an operating system on a Virtual Machine. A VM needs a full guest OS, so I would have to download an ISO, allocate RAM and disk, install the OS, and then configure the web server, which can take around 15 minutes or more. In this lab, pulling the Nginx image and starting the container took only a few seconds because a container shares the host's kernel and packages only the application and its dependencies.

Port mapping with `-p 8080:80` is necessary because a container has its own isolated network. Nginx listens on port 80 inside the container, but that port is not reachable from the host by default. Mapping host port 8080 to container port 80 forwards requests sent to `localhost:8080` into Nginx, which is why curl returned the welcome page.

When I use `docker rm`, the container is deleted together with its writable layer, so any data created inside it is lost unless it was saved in a volume or bind mount. The image itself stays, so a fresh container can be started anytime. This taught me that containers are meant to be disposable.

Containerization also changes how developers and IT operations teams work together. Because an image runs the same everywhere, the "it works on my machine" problem is reduced. Developers package the app once and operations deploy that same image, making releases faster, more consistent, and easier to automate in a DevOps pipeline.

My GitHub portfolio is growing lab by lab. It started with basic Git and Markdown in Laboratory 01 and now includes technical comparisons, documented commands, and screenshot evidence. Committing after every checkpoint is building good documentation habits and a clear record of my progress as a future cloud engineer.
