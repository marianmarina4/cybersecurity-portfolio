# SQL injection UNION attack, retrieving data from other tables

## Objetivo

Realizar un ataque de inyección SQL basado en UNION que recupere todos los nombres de usuario y contraseñas.

## Solución

1. Intercepté la petición con Burp Suite.\
   <img width="604" height="272" alt="image" src="https://github.com/user-attachments/assets/f8bd412d-79af-49bb-a775-8ade400f5b48" />


2. Determiné el número de columnas utilizando `order by` en el parámetro `category`.\
   <img width="364" height="19" alt="image" src="https://github.com/user-attachments/assets/b0dc8b1c-0209-4d85-a624-43033309e668" />


3. Enumeré las tablas de la base de datos con un ataque UNION y luego las columnas.\
   <img width="701" height="20" alt="image" src="https://github.com/user-attachments/assets/9ae9f447-54ef-43a7-a5da-7128976ce650" />\
   <img width="811" height="19" alt="image" src="https://github.com/user-attachments/assets/fb590efd-6382-4858-8b23-61fdc19c1950" />

   
4. Realicé un ataque UNION a las columnas encontradas.\
   <img width="568" height="18" alt="image" src="https://github.com/user-attachments/assets/83c18103-4839-4261-bd46-43888cb4f8df" />


5. Recuperé la información de las columnas encontradas.\
   <img width="179" height="49" alt="image" src="https://github.com/user-attachments/assets/f3088bae-e1d0-4327-81df-4db8b1fa959b" />




## Herramientas utilizadas
- Burp Suite
- Navegador Web
