# Argüello Infancias Mobile

Aplicación móvil para el acompañamiento diario de NNyA en residencias, orientada a educadores y operadores.

## Descripción del proyecto

Argüello Infancias Mobile busca facilitar el registro y la consulta de información relevante durante el acompañamiento cotidiano de niñas, niños y adolescentes (NNyA) en residencias.

La aplicación centraliza información de residentes, novedades, actividades, historial, turnos y situaciones críticas, permitiendo que los educadores accedan a la información necesaria desde una interfaz móvil.

## Problemática

En el trabajo diario dentro de una residencia se genera información que debe registrarse y consultarse de manera clara y organizada. El sistema busca reducir la dispersión de información y facilitar el seguimiento de cada residente, manteniendo criterios de acceso según el rol del usuario.

## Integrantes

- Galvan Camila
- Huansi Jordy
- Melani Lozano
- Martinez Sofia

## Features del proyecto

| Feature | Funcionalidad | Estado |
| --- | --- | --- |
| F1 | Consultar información de residentes asignados | Funcional con datos mock |
| F2 | Registrar novedades | Pendiente; tipos y validaciones preparados |
| F3 | Consultar historial | Vista de solo lectura disponible |
| F4 | Registrar actividades | Pendiente; tipos y validaciones preparados |
| F5 | Consultar turno y tareas | Resumen disponible con datos mock |
| F6 | Reportar situación crítica | Pantalla de advertencia disponible; formulario pendiente |

## Avance actual

El proyecto cuenta con la estructura principal de la aplicación móvil y navegación entre las funcionalidades definidas para el MVP. Actualmente se dispone de pantallas funcionales y datos simulados para validar los principales flujos de uso.

Se encuentran definidos los criterios de aceptación, wireframes, flujos de navegación y documentación de arquitectura del sistema.

## Arquitectura y tecnologías

### Frontend móvil
- Expo SDK 54
- React Native
- TypeScript
- Expo Router
- NativeWind
- Zustand
- Zod

### Backend previsto
- Express.js
- TypeScript
- Supabase Auth
- PostgreSQL

### Herramientas
- Git
- GitHub

## Modelo de datos

El modelo contempla siete tablas principales y relaciones normalizadas hasta Tercera Forma Normal (3FN). También se definieron criterios de integridad referencial e índices para optimizar las consultas.

Antes del despliegue definitivo en Supabase se prevé completar las revisiones de seguridad correspondientes.

## Validaciones realizadas

- 51 criterios de aceptación relevados.
- Verificación de TypeScript sin errores mediante `npx tsc --noEmit`.
- Verificación de lint sin errores.
- `expo-doctor`: 18/18 comprobaciones superadas.
- Validación manual de los principales flujos de navegación.
- Verificación manual de acceso basado en roles (RBAC).

## Próximos pasos

- Completar las funcionalidades pendientes del MVP.
- Implementar los formularios de novedades, actividades y situaciones críticas.
- Integrar el backend con Supabase.
- Aplicar las correcciones de seguridad antes del despliegue.
- Continuar con las pruebas funcionales y validación de los criterios de aceptación.
