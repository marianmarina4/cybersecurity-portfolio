# SQL injection attack, querying the database type and version on Oracle

## Objetivo

Identificar el tipo y la versión de la base de datos utilizada por la aplicación mediante una vulnerabilidad SQL Injection.

## Solución

1. Intercepté la petición utilizando Burp Suite.\
   <img width="466" height="377" alt="image" src="https://github.com/user-attachments/assets/08b797c8-e417-47d2-b528-171fac34ea2b" />

   
2. Modifiqué el parámetro `category` para determinar las columnas utilizando `order by`.\
   <img width="457" height="120" alt="image" src="https://github.com/user-attachments/assets/f78f632c-3be4-4da6-8398-d8b609d66dbb" />

   
3. Utilicé una técnica UNION para recuperar información del sistema gestor de base de datos.\
   <img width="458" height="107" alt="image" src="https://github.com/user-attachments/assets/b0780153-ce17-4a17-9018-bed228f0edfd" />

   
4. Verifiqué que la respuesta mostraba la versión de la base de datos.\
   <img width="1159" height="96" alt="image" src="https://github.com/user-attachments/assets/08f2a068-7962-40ed-8f1b-7c26cec54904" />

## Herramientas utilizadas
- Burp Suite
- Navegador Web
