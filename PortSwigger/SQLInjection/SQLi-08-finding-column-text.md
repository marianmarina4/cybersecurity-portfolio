# SQL injection UNION attack, finding a column containing text

## Objetivo

Realizar un ataque de inyección SQL basado en UNION que devuelva una fila adicional que contenga el valor: 'U7Uefd'.

## Solución

1. Utilicé Burp Suite para interceptar la petición.\
   <img width="631" height="281" alt="image" src="https://github.com/user-attachments/assets/f67ba859-2d8f-464e-9700-975bf41a4abf" />



2. Determiné las columnas utilizando `null` en el parámetro `category`.\
   <img width="525" height="16" alt="image" src="https://github.com/user-attachments/assets/2a29868f-cdac-4f74-aca0-336aeca4cb50" />



3. Testeé el string a devolver en las columnas.\
   <img width="553" height="18" alt="image" src="https://github.com/user-attachments/assets/49237356-a16a-490e-a864-de6dfa8cd82f" />

   
4. Comprobé que la página me devolviera el string insertado.\
   <img width="435" height="65" alt="image" src="https://github.com/user-attachments/assets/a27a1a96-9f4c-4bfa-ade1-4fbaf4f511d4" />




## Herramientas utilizadas
- Burp Suite
- Navegador Web
