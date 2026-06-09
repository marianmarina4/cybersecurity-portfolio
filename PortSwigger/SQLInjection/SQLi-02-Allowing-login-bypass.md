# SQL injection vulnerability allowing login bypass

## Objetivo

Comprender cómo una vulnerabilidad SQL Injection puede ser utilizada para evadir controles de autenticación y obtener acceso a una aplicación sin conocer credenciales válidas.

## Solución

1. Intercepté la solicitud con Burp Suite.
2. Modifiqué el parámetro username 
3. Envié la solicitud.
4. Loguee como administrador.
   

## Evidencias

<img width="604" height="351" alt="image" src="https://github.com/user-attachments/assets/b32cf483-889c-4870-bbb6-b1a1a6f40a4d" />

**Result:**

<img width="736" height="305" alt="image" src="https://github.com/user-attachments/assets/c0bdb663-2271-4a72-a28d-a204c5978f77" />
