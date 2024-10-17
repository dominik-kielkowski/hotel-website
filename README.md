# Hotel Website

A cloud-hosted booking website build with an ASP.NET backend and Angular frontend where users can browse hotels and book rooms. The project is easily deployable to Azure using a Terraform.
A GitHub Actions CI/CD pipeline builds and pushes a Docker image to Docker Hub, from where it gets deployed into Azure Container Apps. The project uses Redis for caching and Azure SQL as the database.
The backend uses Redis Cache in the MediatR pipeline to speed up queries and implements the Unit of Work pattern for atomic transactions. It also includes Unit Tests to ensure code quality.

## Components

- [Hotel Reservation Web Client](https://github.com/dominik-kielkowski/hotel-reservation-web-client)
- [Hotel Reservation API](https://github.com/dominik-kielkowski/hotel-reservation-api)
- [Hotel Reservation Email Service](https://github.com/dominik-kielkowski/hotel-reservation-email-service)
