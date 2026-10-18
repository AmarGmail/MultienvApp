# MultiEnv Ticket Management System using Docker Compose

A full-stack application using Flask for both frontend and backend services, demonstrating environment-specific ticket management.

## Project Structure

```
multienv/
├── docker-compose.yml
├── backend/
│   ├── dev/
│   │   ├── app.py
│   │   ├── requirements.txt
│   │   ├── Dockerfile
│   │   └── .env
│   └── prod/
│       ├── app.py
│       ├── requirements.txt
│       ├── Dockerfile
│       └── .env
└── frontend/
    ├── app.py
    ├── requirements.txt
    ├── Dockerfile
    └── .env
```

Due to time constraint one mongo db container used for both Prod and Dev endpoints.

### Backend Development Deployment

![Development environment](Screentshots/Dev-UI.png)
![Devlopment Service logs](Screentshots/Dev-env-Service-logs.png)
![Development UI via FrontEnd](Screentshots/Dev-Env.png)


### Backend Production Environment 
![Production environment](Screentshots/Production-UI.png)
![Production Service Logs](Screentshots/Prod-Env-Service-logs.png)
![Production env via FrontEnd](Screentshots/Prod-env.png)


### CLI 

```CLI service validation after the deployment
```
![CLI validation](Screentshots/Services-validation.png)

```
docker compose up --build -d
```
![Docker compose build](Screentshots/Docker-Compose-up-build-d.png)

```
docker ps
```
![Docker ps](Screentshots/docker-containers-ps.png)

```
MongoDB deployment logs
```
![MongoDB logs](Screentshots/Mongo-db-logs.png)

```
Production Service logs
```
![Production service logs](Screentshots/Prod-Env-Service-logs.png)

```
Development Service logs
```
![Developemtn Service logs](Screentshots/Dev-env-Service-logs.png)

```
Application FrontEnd
```
![Application ErontEnd](Screentshots/Apps-Frontend.png)
## Accessing the Application

- Frontend: http://localhost:3000/
- Development Environment: http://localhost:3001/dev
- Production Environment: http://localhost:3002/prod






