# SQL injection vulnerability in Where clause allowing retrieval of hidden data

## Objetivo

Comprender cómo una vulnerabilidad SQL Injection puede alterar el comportamiento de una consulta SQL para recuperar datos no previstos por la aplicación.

## Solución

1. Intercepté la solicitud utilizando Burp Suite.
2. Identifiqué el parámetro encargado de filtrar los productos por categoría.
3. Modifiqué dicho parámetro para alterar la consulta SQL.
4. Envié nuevamente la solicitud.
5. Verifiqué que la respuesta mostraba productos que originalmente estaban ocultos.

## Evidencias
<img width="454" height="127" alt="image" src="https://github.com/user-attachments/assets/f1867763-aace-4b59-a4e6-67ad6107e7df" />}


**Result:**

<img width="1199" height="356" alt="image" src="https://github.com/user-attachments/assets/bee95201-c870-40b1-afbd-dcd361899374" />
