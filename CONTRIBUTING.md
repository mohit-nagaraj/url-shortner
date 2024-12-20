# Contributing to URL Shortener

Thank you for considering contributing to our project! Here are some guidelines to help you get started.

## Getting Started
1. **Fork the repository**: Click the "Fork" button at the top of this page to create a copy of the repository under your GitHub account.
2. **Clone the repository**: Use `git clone` to clone the repository to your local machine.
   ```sh
   git clone https://github.com/your-username/url-shortner
   cd url-shortner
   ```
3. **Create a branch**: Create a new branch for your feature or bug fix.
   ```sh
   git checkout -b feature-name
   ```

## Project Structure
- `api/`: Contains the main application logic and routes.
  - `routes.go`: Defines the various API routes.
  - `logic.go`: Contains the core business logic for URL shortening and management.
- `docker/`: Contains Docker-related files for containerization.
- `.env`: Environment configuration file.

## Routes
Below are the primary routes defined in the project:

- `POST /shorten`: Endpoint to create a new shortened URL.
- `GET /:shortURL`: Endpoint to redirect to the original URL.
- `DELETE /:shortURL`: Endpoint to delete a shortened URL.

## Logic
The core logic includes:

- **URL Shortening**: Generates a unique short code for the provided URL and stores it in Redis.
- **Redirection**: Retrieves the original URL from Redis when a short URL is accessed and redirects the user.
- **Expiration**: Manages the expiration of URLs based on predefined criteria.

## Submitting Changes
1. **Commit your changes**: Use descriptive commit messages to explain what you have done.
   ```sh
   git commit -m "Add feature X"
   ```
2. **Push to your branch**: Push your changes to your forked repository.
   ```sh
   git push origin feature-name
   ```
3. **Create a Pull Request**: Navigate to the original repository and create a pull request from your forked repository.

## Code of Conduct
Please adhere to the [Code of Conduct](CODE_OF_CONDUCT.md) when contributing to this project.

## License
By contributing, you agree that your contributions will be licensed under the MIT License.

Thank you for contributing!
