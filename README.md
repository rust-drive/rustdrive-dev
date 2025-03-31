# Development Environment

## Setup

First off all you need to install Docker.
<https://docs.docker.com/get-started/get-docker/>

Then you need vscode or a similar ide.

Recursively clone this Repository.

```bash
git clone --recursive git@github.com:rust-drive/rustdrive-dev.git
```

In the repository run this command, to start the Environment. The firstrun takes a long time to compile.

```bash
docker compose -f development-compose.yaml up
```

## Usage

Start the Environment with this command:

```bash
docker compose -f development-compose.yaml up
```

Stop it with this command:

```bash
docker compose -f development-compose.yaml down
```

These Services will be installed:

- Api Development <http://localhost:9339>
  - User: admin
  - Password: password
- Database Editor <http://localhost:8080>
  - Server: database
  - User: admin
  - Password: cloud-dev-123
- Frontend <http://localhost:80>
  - User: john
  - Password: doe
- Backend <http://localhost:8000>
- Database
