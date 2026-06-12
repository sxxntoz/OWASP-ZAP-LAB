# Detección de Ataques Web OWASP mediante OWASP ZAP (OWASP Top 10)

## Descripción del Proyecto

Este laboratorio tiene como finalidad implementar un entorno de pruebas de seguridad web utilizando aplicaciones vulnerables y la herramienta OWASP ZAP para la detección y análisis de vulnerabilidades pertenecientes al estándar OWASP Top 10.

El proyecto se desarrolla de manera colaborativa mediante GitHub, donde cada integrante cumple un rol específico dentro de un flujo de trabajo secuencial que simula un proceso profesional de auditoría y pentesting web.

---

## Integrantes

| Participante                        | Rol                                                      |
| ----------------------------------- | -------------------------------------------------------- |
| Walter David Mendieta Napan         | Persona 1 – Preparación del entorno y GitHub             |
| Ariana del Rosario Aviles Tolentino | Persona 2 – Configuración y reconocimiento con OWASP ZAP |
| Christian Juica Alarcon             | Persona 3 – Ejecución de pruebas OWASP Top 10            |
| José Fernando Sanchez Guando        | Persona 4 – Análisis, reporte y documentación final      |

---

## Objetivo General

Implementar un laboratorio práctico para la detección de vulnerabilidades web utilizando OWASP ZAP sobre aplicaciones intencionalmente vulnerables, aplicando metodologías de reconocimiento, análisis y documentación de hallazgos.

---

## Objetivos Específicos

* Configurar un entorno de pruebas web seguro y controlado.
* Utilizar GitHub como plataforma colaborativa para la gestión del proyecto.
* Implementar aplicaciones vulnerables para pruebas de seguridad.
* Realizar actividades de reconocimiento mediante OWASP ZAP.
* Detectar vulnerabilidades asociadas al OWASP Top 10.
* Documentar hallazgos técnicos y evidencias.
* Elaborar un informe técnico con los resultados obtenidos.

---

## Herramientas Utilizadas

### Gestión del Proyecto

* Git
* GitHub

### Seguridad Web

* OWASP ZAP

### Aplicaciones Vulnerables

* DVWA (Damn Vulnerable Web Application)
* OWASP Juice Shop
* WebGoat

### Entorno de Ejecución

* Docker Desktop
* WSL2 (Windows Subsystem for Linux)
* Ubuntu

### Sistema Operativo

* Windows 11

---

## Arquitectura del Laboratorio

```text
Walter David Mendieta Napan
(Preparación del entorno y GitHub)
                │
                ▼
Ariana del Rosario Aviles Tolentino
(Config. y reconocimiento con OWASP ZAP)
                │
                ▼
Christian Juica Alarcon
(Ejecución de pruebas OWASP Top 10)
                │
                ▼
José Fernando Sanchez Guando
(Análisis y reporte final)
```

---

## Flujo de Trabajo

### Fase 1

Preparación del entorno de laboratorio:

* Configuración de GitHub.
* Instalación de Docker Desktop.
* Configuración de WSL2.
* Implementación de DVWA.
* Implementación de OWASP Juice Shop.
* Implementación de WebGoat.

### Fase 2

Reconocimiento de aplicaciones web mediante OWASP ZAP:

* Spider Scan.
* Ajax Spider.
* Passive Scan.
* Descubrimiento de recursos y endpoints.

### Fase 3

Detección de vulnerabilidades:

* Active Scan.
* Identificación de vulnerabilidades OWASP Top 10.
* Generación de reportes.

### Fase 4

Análisis y documentación:

* Clasificación de hallazgos.
* Evaluación de riesgos.
* Elaboración del informe final.
* Presentación de resultados.

---

## Estructura del Repositorio

```text
OWASP-ZAP-LAB
│
├── README.md
├── LICENSE
├── .gitignore
│
├── docs
│   └── README.md
│
├── configuracion
│   ├── docker
│   ├── dvwa
│   ├── juiceshop
│   └── webgoat
│
├── evidencias
│   └── capturas
│
├── resultados
│
└── logs
```

---

## Aplicaciones Vulnerables Implementadas

### DVWA

Aplicación web vulnerable diseñada para practicar técnicas de seguridad ofensiva y defensiva.

**URL:**

```text
http://localhost:8080
```

### OWASP Juice Shop

Aplicación vulnerable moderna basada en OWASP Top 10.

**URL:**

```text
http://localhost:3000
```

### WebGoat

Plataforma educativa desarrollada por OWASP para el aprendizaje de seguridad web.

**URL:**

```text
http://localhost:8081/WebGoat
```

---

## Convención de Ramas

```text
main

feature/persona1-entorno

feature/persona2-reconocimiento

feature/persona3-pruebas

feature/persona4-reporte
```

---

## Estado del Proyecto

| Actividad                               | Estado     |
| --------------------------------------- | ---------- |
| Configuración del repositorio           | Completado |
| Implementación del entorno              | Completado |
| Instalación de aplicaciones vulnerables | Completado |
| Reconocimiento con OWASP ZAP            | Pendiente  |
| Pruebas OWASP Top 10                    | Pendiente  |
| Reporte final                           | Pendiente  |

---

## Responsabilidades por Integrante

### Walter David Mendieta Napan (Persona 1)

* Creación del repositorio GitHub.
* Diseño de la estructura del proyecto.
* Instalación y configuración de Docker Desktop.
* Configuración de WSL2 y Ubuntu.
* Implementación de DVWA.
* Implementación de OWASP Juice Shop.
* Implementación de WebGoat.
* Documentación de la instalación del entorno.

### Ariana del Rosario Aviles Tolentino (Persona 2)

* Instalación y configuración de OWASP ZAP.
* Configuración del proxy.
* Spider Scan.
* Ajax Spider.
* Reconocimiento de aplicaciones web.
* Enumeración de recursos y endpoints.

### Christian Juica Alarcon (Persona 3)

* Active Scan.
* Detección de vulnerabilidades.
* Validación de hallazgos.
* Identificación de vulnerabilidades OWASP Top 10.
* Exportación de reportes.

### José Fernando Sanchez Guando (Persona 4)

* Consolidación de resultados.
* Clasificación de vulnerabilidades.
* Elaboración del informe técnico.
* Análisis de riesgos.
* Preparación de la presentación final.

---

## Referencias

* OWASP Top 10
* OWASP ZAP
* DVWA (Damn Vulnerable Web Application)
* OWASP Juice Shop
* WebGoat
* Docker Desktop
* GitHub
