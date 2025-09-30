# Overview
This project was inspired by the Network Chuck video on Open WebUI + LiteLLM. I encourage watching the video for UI set up and overall knowledge.
https://www.youtube.com/watch?v=nQCOTzS5oU0

The project provides a single Docker Compose file for running the following stack:
- PostgreSQL
- LiteLLM
- Open WebUI
- Prometheus
- Nginx

## Quick Start (Insecure)
```bash
sudo git clone https://github.com/danielbherold/openwebui-litellm.git
cd openwebui-litellm
mv .env.example .env
source .env
docker compose up -d
```
- **Open WebUI:** [http://localhost:3000](http://localhost:3000)
- **LiteLLM API:** [http://localhost:4000](http://localhost:4000)
----

# Deployment

## 1. Install Docker & Docker Compose

Follow the official Docker installation guides:

- [Install Docker Engine](https://docs.docker.com/engine/install/)
- [Install Docker Compose Plugin](https://docs.docker.com/compose/install/)
- [Install Docker Compose Plugin From Repository](https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository)

## 2. Clone the Repository
```bash
sudo git clone https://github.com/danielbherold/openwebui-litellm.git
cd openwebui-litellm
```

----
## 3. Configure Environment Variables

Create a `.env` file in the repo root. An example may be found in the `.env.example` file.

## 4. Run Services

Spin up everything in the background:
```bash
source .env
docker compose up -d
```

Check logs:
```bash
docker compose logs -f
```

---

## 5. Access Services

- **Open WebUI:** [http://localhost:3000](http://localhost:3000)
- **LiteLLM API:** [http://localhost:4000](http://localhost:4000)
