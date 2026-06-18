# Guía del Laboratorio

## Detección de Ataques Web OWASP mediante OWASP ZAP (OWASP Top 10)

**Responsable:** Walter David Mendieta Napan

**Rol:** Persona 1 - Preparación del entorno y GitHub

---

# Paso 1. Crear el repositorio en GitHub

## 1.1 Iniciar sesión en GitHub

1. Acceder a https://github.com
2. Iniciar sesión con una cuenta de GitHub.

## 1.2 Crear un nuevo repositorio

1. Hacer clic en **New Repository**.
2. Asignar el nombre:

```text
OWASP-ZAP-LAB
```

3. Seleccionar la opción **Public**.
4. Marcar las opciones:

* Add a README file
* Add .gitignore
* Add License (MIT)

5. Hacer clic en **Create Repository**.

### Evidencia

```text
![Creación del repositorio](../evidencias/capturas/01-repositorio-cread.png)
```

---

# Paso 2. Crear la estructura del proyecto

## 2.1 Crear las carpetas principales

Crear la siguiente estructura dentro del repositorio:



```text
OWASP-ZAP-LAB
│
├── guia-laboratorio
│   └── README.md
│
├── configuracion
│   ├── dvwa
│   │   └── README.md
│   ├── juiceshop
│   │   └── README.md
│   └── webgoat
│       └── README.md
│
├── evidencias
│   └── capturas
│       └── README.md
│
├── resultados
│   └── README.md
│
├── logs
│   └── README.md
│
├── README.md
├── LICENSE
└── .gitignore
```

## 2.2 Confirmar los cambios

1. Guardar la estructura.
2. Realizar Commit Changes.

### Evidencia

```text
02-estructura-repositorio.png
```

---

# Paso 3. Verificar requisitos de virtualización

## 3.1 Abrir el Administrador de tareas

1. Presionar:

```text
Ctrl + Shift + Esc
```

2. Ir a la pestaña:

```text
Rendimiento
```

3. Seleccionar:

```text
CPU
```

4. Verificar que aparezca:

```text
Virtualización: Habilitado
```

### Evidencia

```text
03-verificacion-virtualizacion.png
```

---

# Paso 4. Instalar Docker Desktop

## 4.1 Descargar Docker Desktop

1. Acceder a:

https://www.docker.com/products/docker-desktop/

2. Descargar la versión:

```text
Windows AMD64
```

## 4.2 Ejecutar el instalador

1. Ejecutar el archivo descargado.
2. Seleccionar:

```text
All-users installation
```

3. Continuar con la instalación.

### Evidencia

```text
04-ejecucion-instalador-docker.png
```

---

## 4.3 Reiniciar el sistema

1. Finalizar la instalación.
2. Reiniciar Windows cuando sea solicitado.

### Evidencia

```text
05-instalacion-completa-docker.png
```

---

## 4.4 Instalar WSL2

Al reiniciar el sistema:

1. Docker detectará que WSL no está instalado.
2. Se iniciará automáticamente el proceso de instalación.
3. Esperar la descarga e instalación de Ubuntu.

---

## 4.5 Configurar Ubuntu

1. Crear usuario Linux.

Ejemplo:

```text
Usuario: david
```

2. Crear contraseña.

3. Finalizar la configuración inicial.

---

## 4.6 Verificar Docker

Abrir CMD y ejecutar:

```bash
docker --version
```

Resultado esperado:

```text
Docker version XX.X.X
```

### Evidencia

```text
06-docker-instalado.png
```

---

# Paso 5. Implementar DVWA

## 5.1 Descargar la imagen Docker

Abrir CMD como administrador.

Ejecutar:

```bash
docker pull vulnerables/web-dvwa
```

### Evidencia

```text
07-descargar-imagen-DVWA.png
```

---

## 5.2 Crear el contenedor

Ejecutar:

```bash
docker run -d --name dvwa -p 8080:80 vulnerables/web-dvwa
```

### Evidencia

```text
08-ejecutar-DVWA.png
```

---

## 5.3 Verificar el contenedor

Ejecutar:

```bash
docker ps
```

Debe aparecer:

```text
dvwa
```

### Evidencia

```text
09-dvwa-contenedor-activo.png
```

---

## 5.4 Verificar funcionamiento

Abrir el navegador:

```text
http://localhost:8080
```

### Evidencia

```text
10-dvwa-funcionando.png
```

---

# Paso 6. Implementar OWASP Juice Shop

## 6.1 Descargar la imagen Docker

Ejecutar:

```bash
docker pull bkimminich/juice-shop
```

### Evidencia

```text
11-descargar-juice-shop.png
```

---

## 6.2 Crear el contenedor

Ejecutar:

```bash
docker run -d --name juice-shop -p 3000:3000 bkimminich/juice-shop
```

### Evidencia

```text
12-ejecutar-juice-shop.png
```

---

## 6.3 Verificar el contenedor

Ejecutar:

```bash
docker ps
```

Debe aparecer:

```text
juice-shop
```

### Evidencia

```text
13-juice-contenedor-activo.png
```

---

## 6.4 Verificar funcionamiento

Abrir:

```text
http://localhost:3000
```

### Evidencia

```text
14-juice-funcionando.png
```

---

# Paso 7. Implementar WebGoat

## 7.1 Descargar la imagen Docker

Ejecutar:

```bash
docker pull webgoat/webgoat
```

### Evidencia

```text
15-descargar-webgoat.png
```

---

## 7.2 Crear el contenedor

Ejecutar:

```bash
docker run -d --name webgoat -p 8081:8080 webgoat/webgoat
```

### Evidencia

```text
16-ejecutar-webgoat.png
```

---

## 7.3 Verificar el contenedor

Ejecutar:

```bash
docker ps
```

Debe aparecer:

```text
webgoat
```

### Evidencia

```text
17-webgoat-contenedor-activo.png
```

---

## 7.4 Verificar funcionamiento

Abrir:

```text
http://localhost:8081/WebGoat
```

### Evidencia

```text
18-webgoat-funcionando.png
```

---

# Entregables para la Persona 2

Al finalizar esta fase deben encontrarse disponibles:

* Repositorio GitHub configurado.
* Docker Desktop funcionando correctamente.
* WSL2 instalado.
* DVWA operativo.
* OWASP Juice Shop operativo.
* WebGoat operativo.
* Evidencias documentadas.
* Estructura del proyecto creada.

La Persona 2 podrá utilizar estas aplicaciones para realizar el reconocimiento mediante OWASP ZAP.

