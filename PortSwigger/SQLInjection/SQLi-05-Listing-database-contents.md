# SQL injection attack, listing the database contents on non-Oracle databases

## Objetivo

Utilizar una vulnerabilidad SQL Injection para enumerar la estructura de una base de datos y obtener información sobre sus tablas y columnas.

## Solución

1. Intercepté la petición utilizando Burp Suite.\
   <img width="708" height="296" alt="image" src="https://github.com/user-attachments/assets/2f1701ba-92df-4141-b26e-a35ab29bdf0e" />


2. Modifiqué el parámetro `category` para determinar las columnas utilizando `order by`.\
   <img width="473" height="113" alt="image" src="https://github.com/user-attachments/assets/4fbc9da1-6c22-4e0f-8a93-a3f9f730176a" />


3. Utilicé una técnica UNION para enumerar las tablas disponibles y posteriormente sus columnas.\
   <img width="726" height="22" alt="image" src="https://github.com/user-attachments/assets/efed4bc7-f396-462a-844c-0c60e872895b" />
   <img width="956" height="23" alt="image" src="https://github.com/user-attachments/assets/3a827a1f-cae3-4d10-865a-9ee3182f440a" />


4. Identifiqué columnas relevantes almacenadas en la base de datos y recuperé la información de las mismas.\
   <img width="751" height="15" alt="image" src="https://github.com/user-attachments/assets/be839232-c990-4fed-bdf5-82ab74cb959b" />\
   <img width="171" height="57" alt="image" src="https://github.com/user-attachments/assets/942c8f12-2383-4f26-b08b-fb4ef9ab958e" />



## Herramientas utilizadas
- Burp Suite
- Navegador Web
