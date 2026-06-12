# WebGoat

## Descripción

WebGoat es una plataforma educativa desarrollada por OWASP que permite aprender y practicar vulnerabilidades web mediante ejercicios guiados.

## Objetivo

Implementar WebGoat utilizando Docker para complementar las pruebas de seguridad web realizadas con OWASP ZAP.

## Requisitos

* Docker Desktop
* WSL2 configurado
* Conexión a Internet

## Descarga de la imagen

```bash
docker pull webgoat/webgoat
```

## Ejecución del contenedor

```bash
docker run -d --name webgoat -p 8081:8080 webgoat/webgoat
```

## Verificación

Verificar que el contenedor se encuentre activo:

```bash
docker ps
```

Resultado esperado:

```text
webgoat/webgoat
```

## Acceso a la aplicación

Abrir en el navegador:

```text
http://localhost:8081/WebGoat
```

## Observación

La primera carga puede tardar entre 1 y 3 minutos debido a la inicialización de los servicios Java.

## Evidencias requeridas

* Descarga de la imagen Docker.
* Contenedor en ejecución.
* Pantalla de inicio de sesión de WebGoat.

## Responsable

David Mendieta – Preparación del entorno y GitHub.
