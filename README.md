# CineNest.ai

 CineNest.ai is an ai integrated film production system which aims to Transform film making into a fully automated , transparent  and efficient  Environment

## Team
- **Adhil Rifayin k s** — Team Lead  — 007rifayinadhil@gmail.comm
- **Deethu p** — Full Stack Developer — deethup911@gmail.com
- **Abhinav p** — AI Automation Specialist — abhinavvkd10@gmail.com
- **Muhammed Fahad E V** — AI Automation Specialist — fahadman40@gmail.com


## Requirements (Repository checklist)
This repository follows the required structure for the competition.

## How to run locally (Docker)
1. Install Docker & Docker Compose.
2. Copy `.env.example` to `.env` and set environment variables.
3. Start services:
```bash
docker-compose up --build
```


### Pull the Node.js Docker image:
docker pull node:22-alpine

### Create a Node.js container and start a Shell session:
'docker run -it --rm --entrypoint sh node:22-alpine

### Verify the Node.js version:
node -v' #### Should print "v22.20.0"

### Verify npm version:
npm -v
#### Should print "10.9.3"


##Make sure Node.js is installed:
node -v
npm -v

##Install Firebase CLI
##Use npm to install Firebase tools globally:
npm install -g firebase-tools

##Login to Firebase
##You need to authenticate your Google account:
firebase login


4. Open the app / n8n at the URL printed in the compose logs (by default configured below).

## How to run tests
```bash
# placeholder for unit tests
pytest
```

## Deployment (Local Docker)
See `deployment/docker-compose.yml` and `deployment/Dockerfile` for local deployment instructions.


# n8n Workflow Helper Scripts

Helper scripts for automating n8n workflow startup and database seeding, suitable for pipeline management in VFX/automation studios.

## Features

- start-workflow.sh: Launches an n8n workflow via HTTP webhook.
- seed-db.sql: Seeds Postgres/MySQL database with sample data for workflow development.
- Easily customize endpoints and payloads for your environment.

## Usage

- Edit endpoints and credentials in start-workflow.sh as needed.
- Run seed script via your database CLI:
## Environment variables (example)
- POSTGRES_USER
- POSTGRES_PASSWORD
- POSTGRES_DB
- N8N_BASIC_AUTH_ACTIVE
- N8N_BASIC_AUTH_USER
- N8N_BASIC_AUTH_PASSWORD

## Known limitations & TODOs
- This repository contains a starter n8n workflow and scaffolding. Connect real credentials before use.
- TODO: Add unit tests for backend modules.
- TODO: Add Kubernetes manifests (if deploying to k8s).

## License & Attributions
Licensed under the MIT License — see `LICENSE` for details.
