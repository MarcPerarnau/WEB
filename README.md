# 📌 Proyecto: Página Básica con Formulario y Base de Datos MySQL

Este repositorio contiene una página web básica con un pequeño formulario que almacena datos en una base de datos `MySQL`. La aplicación se ejecuta con `docker-compose`, utilizando `Nginx` como servidor web y `PHP` como backend.

## 📂 Estructura del Proyecto
```
.
├── docker-compose.yaml       
├── LICENSE                   
├── mysql
│   └── script.sql            
├── nginx
│   ├── Dockerfile            
│   └── nginx.conf            
├── php
│   ├── Dockerfile            
│   └── index.php             
├── README.md                 
└── REAMDE.md                 

```
## 🚀 Despliegue

### 📋 Requisitos Previos

Asegúrate de tener instalados los siguientes programas en tu sistema: 

- Docker
- Docker Compose

### 🔧 Instalación y Ejecución

1. Clona el repositorio:
```
git clone https://github.com/MarcPerarnau/Web.git
cd web
```
2. Inicia los contonedores con `docker-compose`:
```
docker-compose up -d
```
3. Accede a la aplicación en tu navegador: 
```
http://localhost:8080
```
4. Para detener los contonedores: 
```
docker-compose down
```

## 🛠 Configuración de Servicios

### 📌 Nginx

- Configurado en `nginx/nginx.conf`
- Servidor proxy inverso para php

### 📌 PHP

- Código en php/index.php
- Procesamiento de formularios y conexión a MySQL

### 📌 MySQL

- Script de creación en mysql/script.sql
- Se ejecuta automáticamente al iniciar el contenedor

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Sigue estos pasos para colaborar:
1. Fork el repositorio
2. Crea una nueva rama con tu funcionalidad o correción:
```
git checkout -b mi-nueva-funcionalidad
```
3. Realiza los cambios y haz un commit:
```
git commit -m "Añadida nueva funcionalidad"
```
4. Sube los cambios a tu fork:
```
git push origin mi-nueva-funcionalidad
```
5. Abre un Pull Request en este repositorio.

## 📌 Autor y Contribuidores

- Autor: [Marc Perarnau (DevLab)](http://github.com/MarcPerarnau)
- Contribuidores: Agrega tu nombre aquí cuando contribuyas 🎉

## 📜 Licencia

Este proyecto se distribuye bajo la licencia MIT.
