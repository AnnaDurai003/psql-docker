# PostgreSQL and pgAdmin Docker Setup

This repository contains a `docker-compose.yml` file that sets up a PostgreSQL database and pgAdmin using Docker. This setup allows you to manage your PostgreSQL databases and interact with them through a web-based GUI.

## Prerequisites

Before you begin, ensure you have the following installed on your machine:

- Docker: [Install Docker](https://docs.docker.com/get-docker/)
- Docker Compose: [Install Docker Compose](https://docs.docker.com/compose/install/)

## Getting Started

Follow these steps to set up and run PostgreSQL and pgAdmin using Docker.

### 1. Clone the Repository

Clone this repository to your local machine:

```sh
git clone https://github.com/AnnaDurai003/psql-docker.git
```
```sh
cd psql-docker
```

### 2. Start the Docker Services

Open a terminal and navigate to the directory containing your docker-compose.yml file. Run the following command to start the services
 
```sh
docker-compose up -d
```
This command will start PostgreSQL and pgAdmin in detached mode.

### 3. Access pgAdmin
Open your web browser and go to http://localhost:5050.

Log in using the email and password provided in the docker-compose.yml file:
- Email: ``` admin@email.com ```
- Password: ``` admin ```

### 4. Connect pgAdmin to PostgreSQL
After logging into pgAdmin, you need to add a new server to connect to your PostgreSQL instance:
- Click on "Add New Server".
- Under the "General" tab, give your server a name.
- Under the "Connection" tab, fill in the details:
    - Hostname: ```postgres```
    - Port: ```5432```
    - Username: ```postgres```
    - Password: ```postgres```