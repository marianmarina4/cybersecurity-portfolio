# SQL injection vulnerability in Where clause allowing retrieval of hidden data

## Objetivo

Comprender cómo una SQL Injection puede utilizarse para evadir mecanismos de autenticación.

## Conceptos

- Authentication Bypass
- SQL Injection
- Input Validation

## Metodología

1. Identificación del punto de entrada.
2. Pruebas de caracteres especiales.
3. Confirmación de SQL Injection.
4. Bypass de autenticación.

## Evidencias

(Capturas propias)

## Impacto

Un atacante podría acceder a cuentas sin conocer credenciales válidas.

## Mitigación

- Consultas parametrizadas.
- ORM.
- Validación de entradas.

## Aprendizajes

- Cómo detectar una SQLi en formularios de login.
- Cómo interpretar mensajes de error.
