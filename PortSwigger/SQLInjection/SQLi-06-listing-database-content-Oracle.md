# SQL injection attack, listing the database contents on Oracle

## Objetivo

Utilizar una vulnerabilidad SQL Injection para enumerar la estructura de una base de datos Oracle y obtener información sobre sus tablas y columnas.

## Solución

1. Intercepté la petición utilizando Burp Suite.\
   <img width="617" height="275" alt="image" src="https://github.com/user-attachments/assets/d4071423-0f32-43e4-b60f-63b7b6de7ea9" />



2. Determiné las columnas utilizando `order by` en el parámetro `category`.\
   <img width="394" height="24" alt="image" src="https://github.com/user-attachments/assets/3209f5d6-58bd-415d-9b55-96779fb907c0" />


3. Utilicé una técnica UNION para enumerar las tablas de la base de datos y posteriormente sus columnas.\
   <img width="611" height="20" alt="image" src="https://github.com/user-attachments/assets/d58d4f3d-e22f-4b91-80eb-22f8fc21e51e" />

   
4. Enumeré las columnas de las tabla users con la misma técnica.\
   <img width="874" height="17" alt="image" src="https://github.com/user-attachments/assets/5c2759f7-6f17-49d1-b66a-b598803da639" />


5. Identifiqué columnas relevantes almacenadas en la base de datos y recuperé la información de las mismas.\
   <img width="738" height="25" alt="image" src="https://github.com/user-attachments/assets/bdbe3d20-2311-454a-87f9-7dc1062bd798" />\
   <img width="191" height="54" alt="image" src="https://github.com/user-attachments/assets/15752533-81c1-4f0b-993a-2394425903dd" />


## Herramientas utilizadas
- Burp Suite
- Navegador Web
