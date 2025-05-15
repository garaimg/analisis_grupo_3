# 📊 Análisis de Estudiantes – Grupo 3

Este proyecto contiene un análisis exploratorio de datos de estudiantes utilizando Python y Jupyter Notebook, todo contenido en un entorno Dockerizado para facilitar su ejecución.

---

## 📁 Estructura del proyecto

```
.
├── README.md
├── analisis_estudiantes.ipynb
├── docker-compose.yml
└── jupyter
    ├── Dockerfile
    └── requirements.txt
```

---

## 🚀 Instrucciones de uso

### 1. 🐳 Requisitos previos

Asegúrate de tener instalado:

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

---

### 2. ▶️ Ejecutar Jupyter Notebook

Abre una terminal en el directorio raíz del proyecto y ejecuta:

```bash
docker-compose up --build
```

Esto hará lo siguiente:

- Construirá la imagen de Docker usando `jupyter/Dockerfile`.
- Instalará las dependencias desde `jupyter/requirements.txt`.
- Levantará un contenedor con Jupyter Notebook accesible desde tu navegador.

---

### 3. 🌐 Acceder a Jupyter

Una vez el contenedor esté levantado, abre tu navegador y ve a:

```
http://localhost:8888
```

El token de autenticación está deshabilitado, por lo que accederás directamente al entorno.

---

### 4. 🛑 Detener el contenedor

Presiona `Ctrl+C` en la terminal para detener el contenedor, o bien:

```bash
docker-compose down
```

---

## ✅ Notas

- Todos los archivos del proyecto se encuentran en la carpeta `work` dentro del contenedor.
- Para añadir más dependencias, edita `jupyter/requirements.txt` y vuelve a ejecutar `docker-compose up --build`.

---