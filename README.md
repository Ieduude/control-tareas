# Control de Tareas

## Descripción

Este proyecto consiste en una aplicación sencilla para llevar el control de tareas personales. Cada tarea tiene un ID, título, descripción, prioridad y un estado que indica si está completada o pendiente.

El proyecto se realizó para practicar **Java, Maven, HTTP y REST**, diseñando la estructura de una API de control de tareas.

## Tecnologías utilizadas

* Java 17
* Maven
* IntelliJ IDEA
* HTTP
* REST
* JSON
* Git y GitHub

## Datos del proyecto

* **GroupId:** `com.estudiante`
* **ArtifactId:** `control-tareas`
* **Versión:** `1.0-SNAPSHOT`
* **Java:** 17

## Estructura

```text
control-tareas/
├── src/
│   ├── main/
│   │   └── java/
│   │       └── com/
│   │           └── estudiante/
│   │               ├── Tarea.java
│   │               └── Main.java
├── evidencias/
├── pom.xml
├── README.md
└── .gitignore
```

## Maven

Se utilizaron los siguientes comandos para comprobar que el proyecto funcionara correctamente:

```bash
mvn clean
mvn compile
mvn test
mvn package
```

El comando `package` genera el archivo `.jar` dentro de la carpeta `target`.

## Endpoints REST

| Operación       | Método | Endpoint           |
| --------------- | ------ | ------------------ |
| Consultar todas | GET    | `/api/tareas`      |
| Consultar una   | GET    | `/api/tareas/{id}` |
| Registrar       | POST   | `/api/tareas`      |
| Modificar       | PUT    | `/api/tareas/{id}` |
| Eliminar        | DELETE | `/api/tareas/{id}` |

## Ejemplo JSON

```json
{
  "id": 1,
  "titulo": "Comprar alimentos",
  "descripcion": "Comprar productos para la semana",
  "prioridad": "ALTA",
  "completada": false
}
```

## Autor

**Nombre:** Iván Eduardo del Cid Véliz
**Carné:** `9941-25-20822`
