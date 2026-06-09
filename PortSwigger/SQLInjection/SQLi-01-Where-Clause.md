# SQL injection vulnerability in Where clause allowing retrieval of hidden data

## Objetivo

Comprender cómo una vulnerabilidad SQL Injection puede alterar el comportamiento de una consulta SQL para recuperar datos no previstos por la aplicación.

## Conceptos
- SQL Injection
- WHERE Clause Manipulation
- Data Exposure
- Input Validation
- Query Logic Manipulation

## Metodología

1. **Identificación del punto de entrada**

   Se identificó un parámetro controlado por el usuario que influía directamente en una consulta realizada por la aplicación.
   
2. **Análisis del comportamiento**

   Se observaron diferencias en las respuestas de la aplicación al modificar el valor del parámetro, indicando una posible interacción insegura con la base de datos.
   
3. **Confirmación de SQL Injection**

   Mediante pruebas controladas se verificó que era posible alterar la lógica de la cláusula WHERE de la consulta SQL.
   
4. **Explotación**

   La vulnerabilidad permitió modificar los criterios de filtrado utilizados por la aplicación, provocando la visualización de registros que normalmente deberían permanecer ocultos.

## Evidencias

(Capturas propias)

## Impacto

Una vulnerabilidad de este tipo puede permitir:

- Exposición de información sensible.
- Acceso a registros restringidos.
- Enumeración de datos internos.
- Bypass de controles de negocio implementados únicamente a nivel de aplicación.

## Mitigación

- Consultas parametrizadas.
- ORM.
- Validación de entradas.
- Aplicación del principio de mínimo privilegio en la base de datos.
- Revisiones periódicas de código y pruebas de seguridad.
