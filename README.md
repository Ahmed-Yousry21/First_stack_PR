# Social Media App Stack Project

This project sets up a complete stack for a social media application using Vagrant to create and manage 5 virtual machines (VMs). The stack includes Nginx, Apache Tomcat, MySQL, Memcached, and RabbitMQ.

## Table of Contents
- [Overview](#overview)
- [Components](#components)
- [Prerequisites](#prerequisites)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Architecture Diagram](#architecture-diagram)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project leverages Vagrant to automate the provisioning of a multi-tier architecture for a social media application. The setup includes VMs for the following components:

- **Nginx**: Web server and reverse proxy
- **Apache Tomcat**: Application server
- **MySQL**: Database server
- **Memcached**: Distributed memory caching system
- **RabbitMQ**: Message broker

## Components

1. **Nginx**: Handles HTTP requests and acts as a reverse proxy to the Tomcat server.
2. **Apache Tomcat**: Serves the Java-based social media application.
3. **MySQL**: Manages the database for user data, posts, comments, etc.
4. **Memcached**: Provides caching to improve the performance of the application.
5. **RabbitMQ**: Manages message queuing for asynchronous processing.

## Prerequisites

Ensure you have the following installed on your local machine:

- Vagrant
- VirtualBox

## Setup Instructions

1. Clone the repository and navigate to the project directory.

2. Initialize the Vagrant environment by running `vagrant up`.

3. Access the VMs using `vagrant ssh` followed by the respective VM name (nginx, tomcat, mysql, memcached, rabbitmq).

4. Verify the setup:
   - Visit the Nginx server at `http://localhost:8080`.
   - Access Tomcat via Nginx reverse proxy.
   - Connect to the MySQL database using a MySQL client.
   - Check the status of Memcached and RabbitMQ services.

## Usage

After starting the VMs, you can start deploying your social media application on the Tomcat server. Ensure your application is configured to connect to the MySQL database, utilize Memcached for caching, and RabbitMQ for message queuing.

## Architecture Diagram

![Architecture Diagram](path/to/your/diagram.png)

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push to the branch.
5. Create a new Pull Request.

