# docker-compose_practice
This is a simple Flask demo app that counts the number of visits to the app and displays the hostname of the container serving the request. The app uses Redis to store the visit count.

## Prerequisites
- Docker
- Docker Compose
## Installation

1. Clone the repository:

```bash
git clone https://github.com/Jason-JoJo/flask-demo.git
```

2. Change to the project directory:

```bash
cd flask-demo
```

3. Build and start the containers:

```bash
docker-compose up -d
```

4. Access the app in your web browser at http://localhost:8080
