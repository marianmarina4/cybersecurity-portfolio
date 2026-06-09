# SQL injection attack, querying the database type and version on Oracle

## Objetivo

Comprender cómo una SQL Injection puede utilizarse para evadir mecanismos de autenticación.

## Conceptos

- SQL Injection
- Database Fingerprinting
- Information Disclosure
- Oracle Database
- Enumeration

## Metodología

1. Identificación del punto de entrada
  Se identificó un parámetro controlado por el usuario que interactuaba directamente con consultas realizadas por la aplicación.
2. Confirmación de la vulnerabilidad
  Las pruebas realizadas permitieron verificar que la aplicación era vulnerable a SQL Injection.
3. Reconocimiento de la base de datos
  Se analizaron las respuestas de la aplicación para determinar el sistema gestor de bases de datos utilizado.
4. Bypass de autenticación
  Una vez identificado el entorno Oracle, se recuperó información relacionada con la versión del motor de base de datos.

## Evidencias

(Capturas propias)

## Impacto

La divulgación de información sobre la base de datos puede permitir a un atacante:

- Identificar tecnologías utilizadas por la organización.
- Adaptar ataques a una versión específica del motor.
- Buscar vulnerabilidades conocidas asociadas al software detectado.
- Mejorar la precisión de fases posteriores de explotación.

Aunque no implica acceso directo a datos sensibles, constituye una etapa importante dentro del proceso de reconocimiento.

## Mitigación

- Consultas parametrizadas.
- Restricción de información expuesta en respuestas de la aplicación.
- Aplicación de controles de validación de entrada.
- Actualización y mantenimiento del sistema gestor de bases de datos.
