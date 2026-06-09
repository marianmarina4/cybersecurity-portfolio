# SQL injection vulnerability allowing login bypass

## Objetivo

Comprender cómo una vulnerabilidad SQL Injection puede ser utilizada para evadir controles de autenticación y obtener acceso a una aplicación sin conocer credenciales válidas.

## Conceptos

- Authentication Bypass
- SQL Injection
- Input Validation

## Metodología

1. Identificación del punto de entrada.
   Se identificó un formulario de autenticación que procesaba entradas proporcionadas por el usuario.
2. Pruebas de caracteres especiales.
   Se realizaron pruebas sobre los campos de autenticación para observar posibles comportamientos indicativos de una interacción insegura con la base de datos.
3. Confirmación de SQL Injection.
   Las respuestas de la aplicación permitieron determinar que los datos ingresados influían directamente en la consulta SQL utilizada para validar credenciales.
4. Bypass de autenticación.
   La vulnerabilidad permitió modificar la lógica de autenticación de la aplicación, logrando el acceso a una cuenta sin disponer de credenciales legítimas.

## Evidencias

(Capturas propias)

## Impacto

Una vulnerabilidad de este tipo puede permitir:

- Acceso no autorizado a cuentas de usuario.
- Suplantación de identidad.
- Escalada de privilegios.
- Compromiso de información sensible.
- Toma de control parcial o total de la aplicación.

En entornos reales, este tipo de vulnerabilidad puede derivar en una brecha de seguridad significativa.

## Mitigación

- Consultas parametrizadas.
- Uso de mecanismos robustos de autenticación.
- Validación y sanitización de entradas.

## Aprendizajes

- Cómo detectar una SQLi en formularios de login.
- Cómo una consulta insegura puede afectar los controles de acceso.
- El impacto que puede tener un bypass de autenticación en una aplicación.
