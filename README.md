# Shared Context AI Middelware

This project aims to create a shared context system between ChatGPT and Claude by Anthropic. For Project Technology Stack Decision-Making Process see [PROJECT_DECISION](PROJECT_DECISION.md)

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction
This project aims to create a shared context system between ChatGPT and Claude by Anthropic. This system allows seamless communication and context sharing between the two AI models, enabling more coherent and context-aware interactions.

## Installation
To install and set up the project using API Platform with Docker, follow these steps:

1. **Clone the repository:**
    ```sh
    git clone https://github.com/soft-cloud-dev/shared-context-ai.git
    cd shared-context-ai
    ```

2. **Set up environment variables:**
    ```sh
    cp .env.example .env
    # Update .env with your configuration
    ```

3. **Build and start the Docker containers:**
    ```sh
    docker-compose up -d --build
    ```

4. **Install dependencies inside the Docker container:**
    ```sh
    docker-compose exec php composer install
    ```

5. **Run database migrations (if applicable):**
    ```sh
    docker-compose exec php bin/console doctrine:migrations:migrate
    ```

6. **Access the application:**
    - API Platform: `http://localhost:8080`
    - Admin Panel (if configured): `http://localhost:8081`

## Usage
For usage instructions, refer to the documentation in the `docs` directory.

## Contributing
We welcome contributions to the project. To contribute, follow these steps:

1. **Fork the repository.**
2. **Create a new branch:**
    ```sh
    git checkout -b feature/your-feature-name
    ```

3. **Make your changes and commit them:**
    ```sh
    git commit -m 'Add some feature'
    ```

4. **Push to the branch:**
    ```sh
    git push origin feature/your-feature-name
    ```

5. **Open a pull request.**

Please ensure that your code adheres to the project's coding standards and includes appropriate tests.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact
If you have any questions or need further assistance, feel free to contact the project maintainers:

Maintainer: [lukasz@softcloud.dev](mailto:lukasz@softcloud.dev)
