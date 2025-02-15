# Typebot

This project provides a Docker setup for running Typebot, an open-source tool designed for building conversational experiences and automating interactions.

## Description

This repository contains Docker configurations to easily deploy Typebot. Typebot is an open-source conversational platform that allows you to create and manage chatbots and automated workflows without writing extensive code.

## Services

- **Typebot**: The main service that runs the Typebot application.
  - **Container Name**: typebot
  - **Image**: typebot/typebot
  - **Ports**: Exposed on port (3000)
  - **Volumes**: Data is persisted in `typebot_data` volume, mapped to `/app/typebot`
  - **Environment Variables**: Loaded from `.env`
  - **Restart Policy**: Always restart the container
  - **Resource Limits**: Memory limit of `1G` and CPU limit of `1`

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/typebot.git
    ```

2. Navigate to the project directory:

    ```bash
    cd typebot
    ```

3. Start the services using Docker Compose:

    ```bash
    docker-compose up -d
    ```

## Usage

- Access Typebot at [http://localhost:3000](http://localhost:3000) to create and manage your conversational experiences.

## Contributing

1. Fork the repository.
2. Create a new branch:

    ```bash
    git checkout -b feature/YourFeature
    ```

3. Make your changes and commit them:

    ```bash
    git commit -m "Add your message"
    ```

4. Push to the branch:

    ```bash
    git push origin feature/YourFeature
    ```

5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
