# 📄 Requerimientos del Sistema

## 1. Sistema

* Nombre del sistema: TechCup
* Objetivo: Gestionar de manera centralizada los torneos de fútbol interprogramas de la Escuela Colombiana de Ingeniería Julio Garavito, permitiendo la administración de torneos, registro de equipos y gestión de inscripciones y pagos de forma simple y segura

## 2. Problema a resolver
Actualmente, la Escuela no cuenta con un sistema centralizado que permita crear torneos con sus reglas e información básica, registrar equipos, procesar y validar pagos de inscripción, consultar equipos inscritos, generar reportes de inscripciones y enviar reportes de pagos en formato JSON a la Decanatura

## 3. Diagrama de Contexto

### 3.1 Diagrama

![Diagrama de Contexto](uml/contextdiagramLab3.png)

### 3.2 Actores

| Actor / Rol                        |          Descripción              |
|------------------------------------|:---------------------------------:|
| Organizador del Torneo             | 	Crea y gestiona torneos, verifica pagos, aprueba inscripciones, administra equipos y genera reportes  |
| Capitán de Equipo                  |  Crea y gestiona su equipo, lo registra en el torneo activo y realiza el pago de inscripción vía PSE   |
| Estudiante                         | Se autentica en la plataforma y consulta información de torneos y equipos |

### 3.3 Sistemas externos

| Sistema                            |                                    Descripción                                        |
|------------------------------------|:-------------------------------------------------------------------------------------:|
| Pasarela de Pagos PSE              | Procesa y valida los pagos de la tarifa de inscripción de los equipos                 |
| Decanatura de Ing. de Sistemas     | Recibe los reportes de ingresos por pagos de inscripción en formato JSON              |

## 4. Alcance del sistema
   
### 4.1 Dentro del sistema

- Autenticación de usuarios mediante usuario y contraseña
- Creación y gestión de torneos (crear, cambiar estado, actualizar información)
- Registro de equipos en el torneo activo y gestión de su información
- Procesamiento y validación de pagos de inscripción a través de PSE
- Generación de reportes de equipos inscritos por torneo
- Generación de reportes de ingresos por inscripciones
- Envío de reportes de pagos en formato JSON a la Decanatura

### 4.2 Fuera del sistema

- Procesamiento bancario de las transacciones (lo hace PSE)
- Gestión de información académica de los estudiantes
- Organización logística del torneo (canchas, arbitraje, calendario de partidos)
- Gestión de resultados deportivos y marcadores

