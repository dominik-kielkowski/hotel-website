# Hotel Website

A cloud-hosted booking website build with an ASP.NET backend and Angular frontend where users can browse hotels and book rooms. The project is easily deployable to Azure using a Terraform.
A GitHub Actions CI/CD pipeline builds and pushes a Docker image to Docker Hub, from where it gets deployed into Azure Container Apps. The project uses Redis for caching and Azure SQL as the database.
The backend uses Redis Cache in the MediatR pipeline to speed up queries and implements the Unit of Work pattern for atomic transactions. It also includes Unit Tests to ensure code quality.

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
cd hotel-reservation
