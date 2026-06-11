# SQL injection vulnerability in Where clause allowing retrieval of hidden data

## Objetivo

Realizar un ataque de inyección SQL que provoque que la aplicación muestre uno o más productos aún no publicados.

## Solución

1. Intercepté la solicitud utilizando Burp Suite.\
   <img width="618" height="286" alt="image" src="https://github.com/user-attachments/assets/80b48d65-b670-4559-ab8a-0bbd44b0c9ba" />

 
2. Identifiqué el parámetro encargado de filtrar los productos por categoría.

 
3. Modifiqué dicho parámetro para alterar la consulta SQL.\
   <img width="483" height="116" alt="image" src="https://github.com/user-attachments/assets/83af2b85-718f-427f-b831-350fed42fde0" />

   
4. Verifiqué que la respuesta mostraba productos que originalmente estaban ocultos.\
   <img width="1176" height="349" alt="image" src="https://github.com/user-attachments/assets/8b64b256-39a6-4c8a-9bf6-ac7c67259263" />

## Herramientas utilizadas
- Burp Suite
- Navegador Web


