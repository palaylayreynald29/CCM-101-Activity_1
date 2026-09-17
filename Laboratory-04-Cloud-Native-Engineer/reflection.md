
# Mission 4 Reflection

This laboratory helped me understand how containerization differs from traditional virtualization and how Docker can simplify the deployment of applications. A Docker container generally starts much faster than a Virtual Machine because a VM needs to boot an entire guest operating system, while a container shares the host operating system kernel. In this activity, the Nginx container could be pulled and started with only a few Docker commands, which demonstrated how quickly a containerized application can be deployed compared with setting up a complete operating system and web server on a VM.

Port mapping is necessary because the Nginx web server runs inside the container and listens on port 80. The command `-p 8080:80` connects port 8080 on the host machine to port 80 inside the container. This allowed me to access the Nginx server by using `curl http://localhost:8080` from the host environment. Without the port mapping, the service running inside the container would not be directly accessible through the host's port 8080.

When `docker rm` is used, the specified container is permanently removed. Any data that exists only in the container's writable storage layer is removed along with the container. This showed me why persistent application data should be stored using Docker volumes or other external storage when it needs to survive container deletion.

Containerization also changes how developers and IT operations teams collaborate. Developers can package applications with their dependencies, while operations teams can use the same container image for testing and deployment. This supports more consistent workflows and contributes to DevOps practices.

Finally, my GitHub portfolio is evolving from simply containing cloud-computing information into a collection of practical technical activities. This laboratory added hands-on experience with Docker, Nginx, container lifecycle management, networking, and technical documentation. It also gave me evidence that I can apply cloud-native concepts in a real command-line environment.
