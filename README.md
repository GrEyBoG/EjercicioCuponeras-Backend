# Proyecto de Prueba de Cuponeras EPM - Backend

## Introducción

Este proyecto se centra en el desarrollo de un sistema backend para la gestión de cuponeras para EPM, utilizando Python con Flask. El objetivo es integrar eficientemente este backend con un frontend que se está desarrollando simultáneamente, el cual incluye diversas interfaces para la interacción del usuario.

## Indicaciones de Desarrollo

### Estructura de Carpetas y Nomenclatura de Archivos

- **Modelos**: `models/{entidad}_model.py`
  - Ejemplo: `models/user_model.py` para los modelos de usuarios.
- **Controladores**: `controllers/{entidad}_controller.py`
  - Ejemplo: `controllers/user_controller.py` para las operaciones CRUD de usuarios.
- **Servicios y Clientes**: `clients/{servicio}_client.py`
  - Ejemplo: `clients/mongodb_client.py` para la conexión a MongoDB.
- **Rutas**: `routes/{entidad}_routes.py`
  - Ejemplo: `routes/user_routes.py` para definir las rutas de acceso a funciones del usuario.

### Objetivos

- Reforzar y aplicar el patrón MVC (Modelo-Vista-Controlador).
- Familiarizarse con la estructura de carpetas y buenas prácticas de programación para la escalabilidad y mantenimiento del código.
- Integrar servicios de Azure para la gestión de datos en la nube con SQL Server.
- Utilizar herramientas de versionamiento como Git para facilitar la colaboración y el desarrollo iterativo.

## Lógica a Desarrollar

### Base de Datos

- **Descripción**: Crear una base de datos relacional en Azure SQL Server adaptada a la gestión de cuponeras, usuarios, y transacciones.
- **Implementación**: Definir esquemas de tablas con relaciones adecuadas para soportar la lógica de negocio, incluyendo índices para optimizar las consultas.

### Autenticación y Gestión de Usuarios

- **Login**: Implementar un sistema de autenticación que soporte verificación de credenciales y gestión de sesiones.
- **Registro de Usuarios**: Permitir a los usuarios crear nuevas cuentas, almacenando de manera segura sus datos.

### Gestión de Facturas

- **Búsqueda de Facturas**: Desarrollar una funcionalidad para buscar facturas usando el número de contrato, y generar un cupón vinculado al cliente.
- **Pago de Facturas**: Implementar la actualización del estado de la factura (pagado/no pagado) en la base de datos.

### Comunicaciones

- **Envío de Facturas por Correo**: Simular el envío de facturas por correo electrónico.
- **Notificaciones**: Implementar un sistema de notificaciones para alertar a los usuarios sobre cambios en el estado de sus facturas o cupones.

### Gestión de facturas

- **Gestión de Cupones**: Crear lógicas para la generación, uso, y vencimiento de cupones basados en las transacciones de los usuarios.
- **Historial de Transacciones**: Permitir a los usuarios consultar su historial de transacciones y cupones generados.

## Herramientas y Tecnologías

- **Lenguajes y Frameworks**: Python, Flask, FastAPI.
- **Base de Datos**: Azure SQL Server.
- **Versionamiento**: Git, con uso de ramas para cada característica y PRs (Pull Requests) para la integración de cambios.
- **Integración con Frontend**: Asegurar que las APIs desarrolladas sean consumibles por el frontend y provean todos los datos necesarios para las interfaces de usuario.

## Contribución y Colaboración

- **Ramas de Desarrollo**: Todos los colaboradores deben crear y utilizar ramas individuales para nuevas características o cambios, nunca directamente en `main`.
- **Pull Requests y Revisiones**: Todos los cambios deben ser revisados antes de su integración.
- **Comunicación**: Mantener una comunicación clara y constante con el equipo de frontend para asegurar que el backend cumpla con los requisitos y expectativas del proyecto.

## Notas Adicionales

Este proyecto no solo busca desarrollar habilidades técnicas en las tecnologías mencionadas, sino también mejorar las habilidades de colaboración y gestión de proyectos en un entorno real de desarrollo
