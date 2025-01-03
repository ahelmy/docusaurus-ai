# Docusaurus AI assisstance
This is a simple AI assistance for Docusaurus generated documentation. It is a simple chatbot that can answer questions about your docs.

## Screenshots
![Screenshot](./assets/screenshots/demo.png)


## Architecture
![Architecture](./assets/architecture.png)

## Installation
To install the AI assisstance, you need to clone the repository and install the dependencies. You can do this by running the following commands:
```bash
git clone https://github.com/ahelmy/docusaurus-ai.git
cd docusaurus-ai
yarn install
```


## Run on Docker
1. Run `touch .env` add environment variable for Google Gemine API key if you want, otherwise comment out line 22-26 in `docker-compose.yml`.
2. Run `docker-compose up -d ollama` and wait to be ready.
3. Run `docker-compose exec ollama bash -c "ollama pull llama3.2:1b"` and wait to be ready.
4. Run `docker-compose up -d --build`
5. Open your browser and navigate to `https://docusaurus-ai.localhost` and test the AI assistant.