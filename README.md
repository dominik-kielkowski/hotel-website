# Hotel Website

A cloud-hosted booking website built with an ASP.NET backend and Angular frontend, allowing users to browse hotels and book rooms. The project is easily deployable to Azure using Terraform.
A GitHub Actions CI/CD pipeline builds and pushes a Docker image to Docker Hub, from where the production version is available for deployment in Azure Container Apps, while the local version is used for development and testing using Docker Compose.
The backend uses Redis Cache in the MediatR pipeline to speed up queries and Azure SQL for data storage. It also implements the Unit of Work pattern for atomic transactions and includes Unit Tests to ensure code quality.

## Components

- [Hotel Reservation Web Client](https://github.com/dominik-kielkowski/hotel-reservation-web-client)
- [Hotel Reservation API](https://github.com/dominik-kielkowski/hotel-reservation-api)
- [Hotel Reservation Email Service](https://github.com/dominik-kielkowski/hotel-reservation-email-service)

## Prerequisites

Ensure you have the following installed:

- **Docker**: Download and install from [Docker's official website](https://www.docker.com/products/docker-desktop).

## Clone the Repository

Clone the repository to your local machine:

```bash
git clone https://github.com/dominik-kielkowski/hotel-reservation.git

# Navigate to the directory containing docker-compose.yml
docker-compose up --build
```

## Note

As of October 21st, due to my main focus being on backend and DevOps, not all features have been implemented on the frontend side yet.
The project is updated on a daily basis to add new functionalities.
