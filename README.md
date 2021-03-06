# Brief description

Simplifies the Docker part of [QUARKUS - USING OPENID CONNECT TO PROTECT WEB APPLICATIONS](https://quarkus.io/guides/security-openid-connect-web-authentication).

## Customize Keycloak
In **docker-compose.yml** it's possible to customize Keycloak changing enviroment variables below:
* **KEYCLOAK_USER**=*Your custom user here* (default: **admin**)
* **KEYCLOAK_PASSWORD**=*Your custom password here* (default: **admin**)

You can also change server port and container name inside **docker-compose.yml**. By default, values are respectively: **8180** and **keycloak**.

## Starting Keycloak

To start Keycloak container, locate the folder containing **docker-compose.yml** and execute the command:
```sh
docker-compose up -d
```

You can check if container is up running, using command:
```sh
docker ps
```

The server will running on: http://localhost:8180/auth

## Stopping Keycloak

To stop container, at the same folder, just run:
```sh
docker-compose down
```