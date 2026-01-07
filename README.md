# Portal Docente – Backend

Backend del **Portal de Docentes**, desarrollado como parte de un proyecto de tesis para la Universidad de Sonsonate. Proporciona una API REST para la gestión académica universitaria, soportando autenticación, control de acceso por roles y operaciones sobre datos académicos.

## Tecnologías
- **Node.js**
- **Express**
- **MySQL**

## Descripción

Este backend expone servicios REST que permiten a **docentes y decanos** gestionar grupos, estudiantes, evaluaciones y solicitudes académicas. Implementa **roles diferenciados**, validación de datos y comunicación segura con la base de datos, sirviendo como núcleo lógico del sistema.

## Arquitectura
- API REST
- Separación por capas (rutas, controladores y modelos)
- Persistencia de datos en MySQL

## Estructura del Proyecto

```
Docente-v1/
├── .gitignore
├── ecosystem.config.js
├── index.js
├── package.json
├── package-lock.json
├── src/
│   ├── config/
│   │   └── multerConfig.js
│   ├── controllers/
│   │   ├── configuracion/
│   │   │   └── configuracion.controller.js
│   │   ├── dashboardController/
│   │   │   └── dashboardController.Controller.js
│   │   ├── dataGestion/
│   │   │   └── gestionarCuadro.controller.js
│   │   ├── decanos/
│   │   │   └── decanos.controller.js
│   │   ├── estudiantes/
│   │   │   └── estudiantes.controller.js
│   │   ├── evaluaciones/
│   │   │   └── evaluaciones.controller.js
│   │   ├── facultades/
│   │   │   └── facultades.controller.js
│   │   ├── grupos/
│   │   │   └── grupos.controller.js
│   │   ├── lanzamientos/
│   │   │   └── lanzamientos.controller.js
│   │   ├── loginJWT/
│   │   │   └── login.controller.js
│   │   ├── mantenimiento/
│   │   │   └── mantenimiento.controller.js
│   │   ├── notificaciones/
│   │   │   └── notificaciones.controller.js
│   │   ├── perfil_docente/
│   │   │   └── perfil_docente.controller.js
│   │   ├── posgrado/
│   │   │   └── posgrado.controller.js
│   │   ├── reportes/
│   │   │   └── reportes.controller.js
│   │   └── solicitudes/
│   │       └── solicitudes.controller.js
│   ├── database/
│   │   └── config.js
│   ├── midlewares/
│   │   ├── authMiddleware/
│   │   │   ├── authMiddleware.js
│   │   │   ├── groups.js
│   │   │   └── userData.js
│   │   ├── evaluacionMiddleware/
│   │   │   └── evaluacionMiddleware.js
│   │   ├── uploads/
│   │   │   ├── imageUploadMiddleware.js
│   │   │   └── upload.js
│   │   └── validators/
│   │       └── notes.validator.js
│   ├── routes/
│   │   ├── index.js
│   │   ├── configuracion/
│   │   │   └── configuracion.routes.js
│   │   ├── decanos/
│   │   │   └── decanos.routes.js
│   │   ├── estudiantes/
│   │   │   └── estudiantes.routes.js
│   │   ├── evaluaciones/
│   │   │   └── evaluaciones.routes.js
│   │   ├── facultades/
│   │   │   └── facultades.routes.js
│   │   ├── gestionarCuadro/
│   │   │   └── gestionarCuadro.routes.js
│   │   ├── grupos/
│   │   │   └── grupos.routes.js
│   │   ├── lanzamientos/
│   │   │   └── lanzamientos.routes.js
│   │   ├── loginJWT/
│   │   │   └── login.routes.js
│   │   ├── logout/
│   │   │   └── logout.routes.js
│   │   ├── mantenimiento/
│   │   │   └── mantenimiento.routes.js
│   │   ├── notificaciones/
│   │   │   └── notificaciones.routes.js
│   │   ├── perfil_docente/
│   │   │   └── perfil_docente.routes.js
│   │   ├── posgrado/
│   │   │   └── posgrado.routes.js
│   │   ├── protected/
│   │   │   └── protected.routes.js
│   │   ├── reportes/
│   │   │   └── reportes.routes.js
│   │   └── solicitudes/
│   │       └── solicitudes.routes.js
│   └── utils/
│       └── jwt/
│           └── jwt.js
└── uploads/
```

## Notas
- Proyecto académico desarrollado en un entorno colaborativo
- Enfocado en mantener una estructura clara, escalable y mantenible
