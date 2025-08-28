# MVP Test Workmate

Este repositorio contiene dos proyectos principales: un frontend desarrollado con Angular y un backend desarrollado con NestJS. Ambos proyectos están diseñados para funcionar de manera conjunta como una aplicación de prueba de concepto (MVP) para Workmate.

## mvp_test_frontend (Angular)

La carpeta `mvp_test_frontend` contiene la aplicación cliente construida con Angular. Esta aplicación proporciona la interfaz de usuario para interactuar con el backend y mostrar la información a los usuarios.

### Características Principales:

- **Autenticación**: Gestión de usuarios y sesiones.
- **Visualización de Productos**: Interfaz para explorar y ver detalles de productos.
- **Gestión de Carrito**: Funcionalidad para agregar, eliminar y actualizar productos en un carrito de compras.
- **Checkout**: Proceso para finalizar la compra.

### Cómo Ejecutar el Frontend:

1.  Navega a la carpeta `mvp_test_frontend`:
    ```bash
    cd mvp_test_frontend
    ```
2.  Instala las dependencias:
    ```bash
    npm install
    ```
3.  Inicia el servidor de desarrollo:
    ```bash
    ng serve
    ```
    La aplicación estará disponible en `http://localhost:4200/`.

## mvp-test-backend (NestJS)

La carpeta `mvp-test-backend` contiene la aplicación del servidor construida con NestJS. Este backend expone una API RESTful que es consumida por el frontend, gestionando la lógica de negocio, la base de datos y la autenticación.

### Características Principales:

- **Autenticación y Autorización**: Gestión de usuarios, roles y protección de rutas.
- **API de Productos**: Endpoints para CRUD de productos.
- **API de Usuarios**: Endpoints para gestión de usuarios.
- **Base de Datos**: Integración con una base de datos (se requiere configurar las credenciales).

### Cómo Ejecutar el Backend:

1.  Navega a la carpeta `mvp-test-backend`:
    ```bash
    cd mvp-test-backend
    ```
2.  Instala las dependencias:
    ```bash
    npm install
    ```
3.  Configura las variables de entorno (por ejemplo, para la conexión a la base de datos). Puedes crear un archivo `.env` basado en un `.env.example` si existe.
4.  Inicia la aplicación en modo desarrollo:
    ```bash
    npm run start:dev
    ```
    El servidor estará escuchando en `http://localhost:3000/` (o el puerto configurado).

## Configuración de la Base de Datos

El backend utiliza una base de datos. Asegúrate de configurar las credenciales de la base de datos en el archivo de configuración correspondiente (ej. `.env`). El archivo `database-setup.sql` en la raíz del backend puede usarse para configurar el esquema inicial de la base de datos.

## Estructura del Proyecto

```
.
├── mvp_test_frontend/          # Aplicación frontend de Angular
├── mvp-test-backend/           # Aplicación backend de NestJS
└── README.md                   # Este archivo
```

---

Este `README.md` proporciona una visión general del proyecto y las instrucciones básicas para poner en marcha tanto el frontend como el backend.
