# SQL injection vulnerability allowing login bypass

## Objetivo

Comprender cómo una vulnerabilidad SQL Injection puede ser utilizada para evadir controles de autenticación y obtener acceso a una aplicación sin conocer credenciales válidas.

## Solución

1. Intercepté la solicitud con Burp Suite.\
   <img width="626" height="353" alt="image" src="https://github.com/user-attachments/assets/61f8037b-a604-4adc-b615-b1a09beee3b7" />


2. Modifiqué el parámetro username.\
   <img width="548" height="33" alt="image" src="https://github.com/user-attachments/assets/bc1a2209-9630-42f7-ab35-d1210a3848ce" />


3. Loguee como administrador.\
   <img width="736" height="305" alt="image" src="https://github.com/user-attachments/assets/c0bdb663-2271-4a72-a28d-a204c5978f77" />


## Herramientas utilizadas
- Burp Suite
- Navegador Web
