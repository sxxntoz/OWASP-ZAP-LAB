# DVWA (Damn Vulnerable Web Application)

## Descripción

DVWA es una aplicación web vulnerable diseñada para aprender, practicar y evaluar técnicas de seguridad web en un entorno controlado.

## Objetivo

Implementar DVWA mediante Docker para realizar pruebas de detección de vulnerabilidades utilizando OWASP ZAP.

## Requisitos

* Docker Desktop
* WSL2 configurado
* Conexión a Internet

## Descarga de la imagen

```bash
docker pull vulnerables/web-dvwa
```

## Ejecución del contenedor

```bash
docker run -d --name dvwa -p 8080:80 vulnerables/web-dvwa
```

## Verificación

Comprobar que el contenedor se encuentra en ejecución:

```bash
docker ps
```

Resultado esperado:

```text
vulnerables/web-dvwa
```

## Acceso a la aplicación

Abrir en el navegador:

```text
http://localhost:8080
```

## Credenciales predeterminadas

Usuario:

```text
admin
```

Contraseña:

```text
password
```

## Evidencias requeridas

* Descarga de la imagen Docker.
* Contenedor en ejecución.
* Pantalla de inicio de sesión de DVWA.

## Responsable

David Mendieta – Preparación del entorno y GitHub.

