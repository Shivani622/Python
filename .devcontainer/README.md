**Dev Containers tutorial**
Running Visual Studio Code in a Docker container using the Dev Containers extension.

Running VS Code inside a Docker container can be useful for many reasons.

# Prerequisites
You need Visual Studio Code installed.

# Install Docker
You need Docker to create and manage your containers.

# Docker Desktop
Download and install Docker Desktop, or an alternative Docker option, like Docker on a remote host or Docker compliant CLI.

# Start Docker
First you need to run the Docker Desktop application to start Docker. Docker might take a few minutes to start. If the whale icon is animated, it is probably still in the process of starting. You can click on the icon to see the status.

![image](https://github.com/Shivani622/Python/assets/107998351/0aff854f-8379-4a9b-98e7-3e8341809664)

# Check Docker
Once Docker is running, you can confirm that everything is working by opening a new terminal window and typing the command to check the version of the Docker:
```
docker --version
```

# Install the extension
![image](https://github.com/Shivani622/Python/assets/107998351/e7a651cd-d78b-4f99-bbec-1b6f68da915f)

# Check installation
![image](https://github.com/Shivani622/Python/assets/107998351/3c2c9b60-0e00-41d1-9544-dda0a5d76900)

![image](https://github.com/Shivani622/Python/assets/107998351/28783eb9-c73e-4b11-8e59-bc6f975b297e)

# To Get the sample
To create a Docker container, open a GitHub repository with a Node.js project.

Open the Command Palette (F1) to run the command Dev Containers: Try a Dev Container Sample... and select the Node sample from the list.
![image](https://github.com/Shivani622/Python/assets/107998351/94e07f7a-7a99-4a0a-80f6-0e2704ee1b02)

```Note: There are other dev container samples such as vscode-remote-try-python or vscode-remote-try-java, but this tutorial will use vscode-remote-try-node.```

# Wait for the container to build
When the window reloads, VS Code will create a container from scratch and clone the sample repository into an isolated container volume. A progress message will provide updates, and it may take some time. Fortunately, since the container will already be present, this step won't be required when you open the folder again.

![image](https://github.com/Shivani622/Python/assets/107998351/c4aba334-8c13-4500-8f1c-cf319b0e0962)

The project folder from your local file system is automatically mapped into the container by VS Code when the container has been constructed.

# Examine the container.
Your remote context should change in the bottom left of the Status bar once the container is started and you are connected:
![image](https://github.com/Shivani622/Python/assets/107998351/05518063-389c-4c5e-b4ba-7ceae7143d86)

# Examine your surroundings
Using specific versions of dependencies that your application requires without affecting your local development environment is one of the benefits of developing in a container.

You can verify that Node.js version 18 is installed in the appropriate container for this tutorial by starting a new terminal. 
```
node --version; npm --version
```
![image](https://github.com/Shivani622/Python/assets/107998351/0fdde90f-27b9-45e6-86c5-be2c21777e54)

# Run the application
Press F5, which will run the application inside the container. Once the process starts, navigate to http://localhost:3000 and you should see the simple Node.js server running!

![image](https://github.com/Shivani622/Python/assets/107998351/fb1a449a-c269-4034-bbcf-5ef446bd3988)
