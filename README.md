# PostgreSQL and pgAdmin Setup with Docker Compose

## Services

This Docker Compose configuration contains two services:

1. **PostgreSQL**: A PostgreSQL database server.
2. **pgAdmin**: A web-based PostgreSQL management tool to manage and monitor PostgreSQL databases.

## Configuration

Here are the configuration details for each service:

### PostgreSQL

- **Port**: `5432`
- **User**: `user`
- **Password**: `user`
- **Data Persistence**: The PostgreSQL data is stored in a Docker volume called `pgdata`, ensuring that data is not lost when the container is restarted or removed.

### pgAdmin

- **Port**: `8888` (Accessible via [http://localhost:8888](http://localhost:8888))
- **Email**: `user@domain.com` (Default login email for pgAdmin)
- **Password**: `user` (Default password for pgAdmin)
- **Data Persistence**: pgAdmin configuration and session data is stored in a Docker volume called `pgadmin`.

## Setup Instructions

1. **Clone the repository** (or place the `docker-compose.yml` file in a desired folder).

2. **Run Docker Compose**:
   Open a terminal in the directory where the `docker-compose.yml` file is located and run the following command:

   ```bash
   docker-compose up -d
