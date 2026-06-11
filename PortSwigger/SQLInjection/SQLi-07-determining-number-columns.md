# SQL injection UNION attack, determining the number of columns returned by the query

## Objetivo

Determinar la cantidad de columnas devueltas por la consulta realizando un ataque de inyección SQL UNION.

## Solución

1. Utilicé Burp Suite para interceptar la petición.\
   <img width="604" height="278" alt="image" src="https://github.com/user-attachments/assets/4ace3fb5-fb06-485e-9c2d-2623d5097509" />


2. Determiné las columnas utilizando `null` en el parámetro `category`.\
   <img width="460" height="20" alt="image" src="https://github.com/user-attachments/assets/f5d74c7d-2078-4dac-b518-2c36d6dd1ac1" />


3. Verifiqué que el lab se completó .\
   <img width="486" height="180" alt="image" src="https://github.com/user-attachments/assets/4d483658-5806-4bb6-898d-5a95a952ce08" />


## Herramientas utilizadas
- Burp Suite
- Navegador Web
