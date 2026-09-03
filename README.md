# Argüello Infancias Mobile.md

## Descripción del proyecto

Argüello Infancias Mobile es una aplicación móvil complementaria al
sistema de gestión de residencias.

Está orientada principalmente a educadores u operadores convivenciales y
busca facilitar la consulta y el registro de información relacionada con
el acompañamiento diario de niños, niñas y adolescentes (NNA) durante el
turno.

## Problemática

Actualmente, el acompañamiento diario requiere consultar y registrar
información relevante de los residentes.

Cuando esta información se encuentra distribuida o se gestiona mediante
registros manuales, puede dificultarse su disponibilidad, organización y
trazabilidad.

La aplicación busca centralizar las principales operaciones que necesita
el educador durante su jornada desde un dispositivo móvil.

## Integrantes

-   Galvan Camila
-   Huansi Jordy
-   Melani Lozano
-   Martinez Sofia

## Features del proyecto

  -----------------------------------------------------------------------
  Feature                 Funcionalidad           Estado
  ----------------------- ----------------------- -----------------------
  F1                      Consultar información   Funcional con datos
                          de residentes asignados mock

  F2                      Registrar novedades del Pendiente - tipos y
                          turno                   validaciones listos

  F3                      Consultar historial de  Vista de solo lectura
                          seguimiento             implementada

  F4                      Registrar actividades   Pendiente - tipos y
                          diarias                 validaciones listos

  F5                      Consultar turno y       Pantalla resumen con
                          tareas de hoy           datos mock

  F6                      Reportar una situación  Pantalla de advertencia
                          crítica                 lista - formulario
                                                  pendiente
  -----------------------------------------------------------------------

## Avance actual

Actualmente se encuentra implementada la estructura inicial de la
aplicación, incluyendo:

-   Navegación principal.
-   Pantallas de Inicio, Residentes, Mi turno, Crítica y Perfil.
-   Componentes reutilizables.
-   Consulta y detalle de residentes.
-   Control de acceso según residentes asignados.
-   Sistema de diseño.
-   Componentes de formulario.
-   Modelo de datos definido y validado.

La Feature F1 se encuentra funcional utilizando datos mock.

También existen avances parciales sobre las Features F3, F5 y F6.

## Arquitectura y tecnologías

La aplicación utiliza actualmente:

-   React Native
-   Expo SDK 54
-   TypeScript
-   Expo Router
-   NativeWind
-   Zustand
-   Zod
-   Git / GitHub

Para la persistencia y autenticación se prevé utilizar:

-   Supabase Auth
-   PostgreSQL

También se encuentra prevista una capa backend/API desarrollada con
Express.js y TypeScript.

## Modelo de datos

Se definieron y validaron las siguientes tablas principales:

-   `perfiles_usuarios`
-   `residentes`
-   `turnos_trabajo`
-   `residentes_turnos`
-   `novedades`
-   `actividades_diarias`
-   `situaciones_criticas`

El modelo fue revisado contra los 51 criterios de aceptación definidos
para las seis Features del MVP.

## Validaciones realizadas

-   TypeScript (`npx tsc --noEmit`): sin errores.
-   `npm run lint`: sin errores.
-   Expo Doctor: 18/18 verificaciones.
-   Prueba manual del flujo principal: correcta.
-   Control de acceso por residentes asignados: verificado.
-   51/51 criterios de aceptación cubiertos por el modelo.

## Próximos pasos

1.  Implementar F2 - Registro de novedades.
2.  Aplicar las correcciones pendientes del modelo de datos.
3.  Desplegar la base de datos en Supabase.
4.  Reemplazar progresivamente los datos mock por datos persistentes.
5.  Implementar la capa backend/API.
6.  Continuar incrementalmente con F3, F4, F5 y F6.
