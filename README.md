# Desplegar Docker Compose

## Prerrequisitos

Antes de comenzar, asegúrate de tener lo siguiente instalado en tu sistema:

- **Docker**

- **Git**
  
- **Acceso a Internet para clonar el repositorio desde GitHub**

## Pasos para desplegar la aplicación

### 1. Clonar el repositorio de GitHub

Ejecuta el siguiente comando para clonar el repositorio que contiene el archivo docker-compose.yml:
```bash
git clone https://github.com/MarcPerarnau/Web.git
```

### 2. Navegar al directorio del proyecto

Accede a la carpeta donde se clonó el repositorio:
```
cd Web
```
### 3. Desplegar la aplicación con Docker Compose

Ejecuta el siguiente comando para iniciar los contenedores definidos en el archivo docker-compose.yml:
```
docker-compose up -d
```

Esto iniciará la aplicación en segundo plano (-d).

### 5. Verificar que los contenedores están en ejecución

Para ver los contenedores en ejecución:
```
docker ps
```

Si necesitas ver todos los contenedores, incluidos los detenidos:
```
docker ps -a
```

### 6. Acceder a la aplicación

Si la aplicación es un servicio web, accede desde un navegador en http://localhost:PUERTO, ajustando el puerto según el archivo docker-compose.yml.

### 7. Detener y eliminar los contenedores

Para detener los contenedores:
```
docker-compose down
```

Esto detendrá y eliminará los contenedores creados por Docker Compose.

Conclusión

Siguiendo estos pasos, cualquier usuario puede desplegar fácilmente una aplicación desde un repositorio de GitHub utilizando Docker Compose. Para más detalles, consulta la documentación oficial de Docker.
