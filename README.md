# Sistema de Gestión de Citas Médicas

Proyecto académico de Ingeniería de Software I de la Universidad Abierta para Adultos (UAPA).

Autor: Luis Miguel Contreras.

## Objetivo
Diseñar un sistema que facilite el registro de pacientes y la organización de citas médicas, permitiendo consultar la disponibilidad de los médicos y administrar los horarios de atención.

## Problema que resuelve
La gestión manual de citas puede provocar confusión en los horarios, pérdida de información y asignación de varias citas para un mismo horario. El sistema busca centralizar la información y mejorar la organización de la atención.

## Funcionalidades principales previstas
- Registro y consulta de pacientes.
- Gestión de médicos.
- Agendamiento de citas.
- Consulta y gestión de horarios disponibles.
- Modificación y cancelación de citas.
- Generación de reportes de citas.

## Arquitectura propuesta
Se propone una arquitectura por capas, organizada en presentación, lógica de negocio y acceso a datos.

- Presentación: muestra las pantallas y recibe las solicitudes del usuario.
- Lógica de negocio: aplica las reglas para registrar pacientes y gestionar citas y horarios.
- Acceso a datos: permite guardar y consultar la información en la base de datos.

Esta separación facilita el mantenimiento y permite realizar ajustes sin concentrar todas las responsabilidades en una sola parte del sistema.

## Organización prevista del frontend y backend

### Frontend
Será la interfaz utilizada por el paciente y la recepcionista. Mostrará formularios, horarios disponibles, citas registradas y mensajes de confirmación o error.

Su responsabilidad será recoger los datos del usuario y presentar los resultados de las solicitudes.

### Backend
Procesará las solicitudes del frontend, validará la información y aplicará las reglas de negocio. También gestionará el acceso a la base de datos y los permisos de los usuarios.

Antes de confirmar una cita, deberá comprobar que el médico tenga disponibilidad y evitar que se reserve dos veces el mismo horario.

### Comunicación
El frontend enviará solicitudes al backend mediante una API utilizando HTTPS y datos en formato JSON. El backend procesará cada solicitud, consultará o actualizará la base de datos y devolverá una respuesta.

Por ejemplo, al solicitar una cita, el frontend enviará los datos del paciente, médico y horario. El backend comprobará la disponibilidad y devolverá la confirmación o un mensaje indicando que el horario ya está ocupado.

Esta organización corresponde al diseño previsto y queda pendiente de implementación.

## Herramientas
- Git y GitHub: control de versiones y almacenamiento de los archivos del proyecto.
- GitHub Issues: seguimiento de tareas, riesgos y mejoras.
- GitHub Projects: organización y seguimiento del avance.
- Visual Paradigm Online: elaboración de modelos UML.
- Microsoft Word y PDF: preparación y presentación de la documentación académica.

## Estado actual
El proyecto se encuentra en la etapa de análisis, diseño y documentación. Durante la asignatura se han trabajado los requisitos, las historias de usuario, los modelos UML, la arquitectura inicial y la planificación de tareas.

Las evidencias técnicas fueron incorporadas al repositorio y su carga quedó registrada en el historial de commits.

La programación del frontend, backend y base de datos, así como las pruebas de funcionamiento, quedan pendientes.

## Organización prevista de las evidencias
- Requisitos e historias de usuario.
- Modelos UML.
- Arquitectura y descripción de componentes.
- Evidencias del tablero y seguimiento de tareas.
- Documentación técnica y nota de versión.

## Registro breve de avances
1. Definición del objetivo, alcance y funcionalidades principales del sistema.
2. Elaboración de requisitos e historias de usuario con criterios de aceptación.
3. Modelado UML de actores, clases y procesos principales.
4. Desarrollo del diseño arquitectónico inicial y distribución de responsabilidades.
5. Organización del seguimiento mediante GitHub Projects e identificación de interesados y necesidades de comunicación.

## Seguimiento del proyecto
Repositorio:
https://github.com/contreraslm29-dotcom/sistema-citas-medicas

Tablero:
https://github.com/users/contreraslm29-dotcom/projects/1

## Próximo paso técnico
Consolidar las evidencias en el repositorio, revisar la coherencia entre los requisitos y los modelos e iniciar la implementación del registro de pacientes y el agendamiento de citas.

## Registro de cambios y avances
1. Se definieron los requisitos funcionales y no funcionales, las historias de usuario y los criterios de aceptación del sistema.
2. Se elaboraron los modelos UML para representar los actores, las clases y los procesos principales.
3. Se propuso una arquitectura por capas, separando presentación, lógica de negocio y acceso a datos.
4. Se organizó el seguimiento del proyecto mediante GitHub Projects y se registraron tareas, riesgos y mejoras en Issues.
5. Se incorporaron las evidencias técnicas al repositorio y se documentaron en el README el sistema y la organización prevista del frontend y backend.
