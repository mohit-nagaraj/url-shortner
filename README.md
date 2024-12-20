# URL Shortener

A URL shortening service built using Go and Redis, designed to create and manage shortened URLs efficiently.

## Features
- **Fast and Reliable:** Leverages Go's performance and Redis' speed for quick URL redirection.
- **Easy to Deploy:** Dockerized setup for straightforward deployment.
- **Scalable:** Designed to handle high traffic and large volumes of URL shortening requests.

## Getting Started

### Prerequisites
- [Docker](https://www.docker.com/get-started) installed on your machine.

### Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/mohit-nagaraj/url-shortner.git
   cd url-shortner
   ```

2. Create a `.env` file in the `api` folder with the following information:
   ```env
   DB_ADDR=""
   DB_PASS=""
   APP_PORT=":xxxx"
   DOMAIN="xxxx:yyyy"
   API_QUOTA=number
   ```

### Running the Project
Start the project using Docker Compose:
```sh
docker-compose up -d
```

## Usage
Once the project is running, you can start creating and managing shortened URLs through the provided API endpoints.

## Contributing
Contributions are welcome! Please fork the repository and open a pull request with your changes.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
