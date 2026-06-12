# OWASP Juice Shop

## Descripción

OWASP Juice Shop es una aplicación web intencionalmente vulnerable que permite realizar pruebas de seguridad basadas en el OWASP Top 10.

## Objetivo

Desplegar OWASP Juice Shop mediante Docker para realizar actividades de reconocimiento y detección de vulnerabilidades utilizando OWASP ZAP.

## Requisitos

* Docker Desktop
* WSL2 configurado
* Conexión a Internet

## Descarga de la imagen

```bash
docker pull bkimminich/juice-shop
```

## Ejecución del contenedor

```bash
docker run -d --name juice-shop -p 3000:3000 bkimminich/juice-shop
```

## Verificación

Verificar que el contenedor esté activo:

```bash
docker ps
```

Resultado esperado:

```text
bkimminich/juice-shop
```

## Acceso a la aplicación

Abrir en el navegador:

```text
http://localhost:3000
```

## Evidencias requeridas

* Descarga de la imagen Docker.
* Contenedor en ejecución.
* Página principal de OWASP Juice Shop.

## Responsable

David Mendieta – Preparación del entorno y GitHub.

