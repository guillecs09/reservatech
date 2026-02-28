# ReservaTech: Aplicación Móvil para la Reserva de Aulas – UNMSM

Proyecto desarrollado como parte del curso de Desarrollo de Sistemas Móviles de la Facultad de Ingeniería de Sistemas e Informática – Universidad Nacional Mayor de San Marcos.

Equipo:
- Chavez Torres, Diego Alonso
- Cuentas Santaria, Guillermo
- Remon Chavarria, Luis Angelo
- Rodriguez Huamani, Lian Miguel

La aplicación permite a estudiantes y docentes reservar aulas y laboratorios de la facultad forma eficiente, reemplazando el proceso manual actual por un sistema centralizado, seguro y rápido.

## Descripción General

El proyecto consiste en una aplicación móvil que permite:
- Reservar aulas disponibles.
- Visualizar horarios en tiempo real.
- Gestionar reservas (crear, cancelar, actualizar).
- Recibir notificaciones sobre cambios o confirmaciones.
- Administrar salones y aprobar solicitudes (panel administrador).

Su objetivo principal es optimizar la gestión de espacios físicos en la facultad, mediante un sistema moderno y accesible.

## Problema Identificado

Antes del desarrollo de la aplicación, la facultad no contaba con un sistema formal de reservas.
Esto generaba:

- Procesos manuales lentos.
- Falta de información sobre disponibilidad.
- Errores y conflictos de horarios.
- Poca eficiencia en el uso de los recursos físicos.

- Además, incluye un modelo de predicción, como valor agregado, para anticipar la demanda de salones.

## Tecnologías Utilizadas

### Frontend

- Flutter
- Arquitectura MVVM

### Backend

- PHP
- MySQL
- Firebase Auth
- Azure
- Tensorflow

### Otros
- Control de versiones con GitHub

## Arquitectura de la Solución
<img width="738" height="387" alt="image" src="https://github.com/user-attachments/assets/956b4fc6-1d41-4b3e-b371-883fa9d587d6" />

La arquitectura se basa en:
- Frontend móvil MVVM
- API REST para manejo de reservas
- Servicios independientes:
  - Autenticación (Firebase)
  - Base de datos (Azure/MySQL)
  - Predicción de demanda
- Administrador web para validación y gestión de salones

## Modelo de datos

<img width="1221" height="587" alt="image" src="https://github.com/user-attachments/assets/53e44c51-c410-4de9-ba1e-56e6fdf6e534" />

- Usuario: estudiantes y docentes
- Reserva: información respectiva a cada reserva realizada
- Salon: número, pabellón, capacidad
- Disponibilidad: horarios disponibles para cada salón
- Estado_Reserva: estados de la reserva (Pendiente, Activa, Pasada y Cancelada)

## Funcionalidades
### Cliente
- Login mediante Firebase
- Buscar salones disponibles
- Reservar espacios
- Visualizar historial
- Cancelar reservas
- Notificaciones automáticas

### Administrador
- Validar reservas
- Registrar nuevos salones
- Gestionar disponibilidad
- CRUD completo de salones y usuarios

## Patrones de Diseño Implementados

- Adapter → Integración de validaciones internas y externas
- Singleton → Gestión centralizada de rutas y APIs
- Mediator → Coordinación de interacción entre componentes

## Galería
Vista Login Cliente

<img width="212" height="413" alt="Imagen1" src="https://github.com/user-attachments/assets/6a8f29d2-c0bf-4c73-ab2f-f1b3b8c720ef" />

Vista Reserva de Salones

<img width="210" height="407" alt="2" src="https://github.com/user-attachments/assets/df7ed842-0c15-46ed-a354-42b21690bb1b" />

Vista Mis Reservas

<img width="214" height="417" alt="3" src="https://github.com/user-attachments/assets/4b1d8e27-4978-4f1e-9e13-69c4036323b1" />
