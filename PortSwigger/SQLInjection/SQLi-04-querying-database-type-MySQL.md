# SQL injection attack, querying the database type and version on MYSQL and Microsoft

## Objetivo

Mostrar el tipo y la versión de la base de datos utilizada por la aplicación mediante una vulnerabilidad SQL Injection.

## Solución

1. Intercepté la petición utilizando Burp Suite.\
   <img width="706" height="292" alt="image" src="https://github.com/user-attachments/assets/19473f27-88cc-4c5b-8848-ed5500060960" />

   
2. Modifiqué el parámetro `category` para determinar las columnas utilizando `order by`.\
   <img width="472" height="113" alt="image" src="https://github.com/user-attachments/assets/1fc06576-5421-44d9-8cf8-6f060fc2f0ec" />


3. Utilicé una técnica UNION para recuperar información del sistema gestor de base de datos.\
   <img width="514" height="24" alt="image" src="https://github.com/user-attachments/assets/b7f5f931-5061-4e73-bbe6-7fb7092b09a5" />


4. Verifiqué que la respuesta mostraba la versión de la base de datos.\
   <img width="192" height="33" alt="image" src="https://github.com/user-attachments/assets/a9f0b89c-e416-4141-a0bc-85138d55058f" />

## Herramientas utilizadas
- Burp Suite
- Navegador Web
