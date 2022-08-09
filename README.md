# maven-project

Simple Maven Project

This project will make Jenkins to pull code form GitHub, build artifact file, push the file to ansible server via SSH, ansible server will control the image creation from the new artifact file, push the newly created image to the docker hub, then ansible will order the docker host to pull the same image and run a container out of it.

![Project](https://user-images.githubusercontent.com/64305358/181210542-9313d4ce-f545-4fdf-9def-a92e17703045.PNG)
