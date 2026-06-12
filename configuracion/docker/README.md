# Instalación de Docker Desktop

## Objetivo

Configurar el entorno necesario para ejecutar aplicaciones vulnerables mediante contenedores Docker.

## Requisitos

* Windows 10 o Windows 11
* Virtualización habilitada en BIOS
* Conexión a Internet
* Permisos de administrador

## Instalación de Docker Desktop

1. Descargar Docker Desktop desde la página oficial.
2. Ejecutar el instalador.
3. Mantener habilitada la opción WSL 2.
4. Reiniciar el equipo si es solicitado.

## Configuración de WSL

Durante la instalación se configuró:

* WSL2
* Ubuntu
* Docker Engine

## Verificación

Ejecutar:

```cmd
docker --version
```

Resultado esperado:

```text
Docker version 29.x.x
```

Verificar contenedores:

```cmd
docker ps
```

Resultado esperado:

```text
CONTAINER ID   IMAGE   COMMAND   CREATED
```

## Evidencias

* Docker Desktop instalado.
* WSL2 configurado.
* Docker Engine Running.
* Comandos docker ejecutados correctamente.

## Responsable

David Mendieta – Preparación del entorno y GitHub.
