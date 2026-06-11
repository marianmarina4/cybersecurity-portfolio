# SQL injection UNION attack, retrieving multiple values in a single column

## Objetivo

Realizar un ataque de inyección SQL basado en UNION que recupere todos los nombres de usuario y contraseñas en una sola columna.

## Solución

1. Intercepté la petición con Burp Suite.\
   <img width="603" height="284" alt="image" src="https://github.com/user-attachments/assets/98390e9f-2d1c-4f7b-a641-00c31f6d68c7" />


2. Determiné el número de columnas utilizando `null`.\
   <img width="447" height="16" alt="image" src="https://github.com/user-attachments/assets/b27fe57b-1f2b-4b81-a4cc-b82f7910b320" />


3. Verifiqué cual columna puede contener texto.\
   <img width="449" height="15" alt="image" src="https://github.com/user-attachments/assets/7fddd20d-519f-47a8-8cd4-4532b03e4124" />

   
4. Realicé un ataque UNION para mostrar la información de administrador.\
   <img width="670" height="18" alt="image" src="https://github.com/user-attachments/assets/cbf1541b-c573-437b-a720-ee1af8c3541e" />


5. Recuperé la información de administrador.\
   <img width="290" height="28" alt="image" src="https://github.com/user-attachments/assets/ed08f9f2-c8e2-45cb-80a5-ff2049c6114f" />



## Herramientas utilizadas
- Burp Suite
- Navegador Web
