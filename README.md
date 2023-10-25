# AuctionApp

### (WORK IN PROGRESS)
AuctionApp is a robust microservices-based application designed for auction management. It includes services for identity management, bidding, searching, and real-time notifications, all powered by a modern tech stack.

<img width="1680" alt="architecture-img" src="https://github.com/guieltorres/Carsties/assets/68649783/e2bc332e-45ed-451f-8baf-e1cecfb8f849">

## Services

### Client Apps:

- **WebApp**: A NextJS-based web application for users.
- **MobileApp**: An app available for both iOS and Android platforms.
- **BFF (Backend For Frontend)**: Tailored API to facilitate communication between client apps and microservices.

### Core Services:

- **Identity-svc**: Manages user identities and provides Secure Token Service (STS).
- **Auction-svc**: Handles the creation, updating, and deletion of auction items.
- **Search-svc**: Offers a search feature over auction items.
- **Bidding-svc**: Manages bidding on auction items.
- **Notification-svc**: Provides real-time notifications using SignalR.

## Infrastructure

- **Databases**: Postgres for identity and auction services; MongoDB for search and bidding services.
- **Event Bus**: Ensures seamless, event-driven communication between services.
- **Gateway & Ingress**: Manages and routes incoming traffic.

## Getting Started

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/guieltorres/Carsties.git
   ```

2. **Set Up Each Service**:

   Navigate to each service's directory and run the code bellow:

    ```bash
   dotnet watch
   ```

4. **Run the Application**:

   You can start all services using Docker (ensure Docker is installed):

   ```bash
   docker-compose up
   ```

## License

This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt) file for details.

---

Feel free to modify this template according to the specifics of your project and the additional sections you'd like to have.
