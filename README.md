# Cybersecurity Labs — Mariano Marina

Repositorio personal de laboratorios, writeups, notas técnicas, scripts y documentación relacionada con pentesting, seguridad ofensiva y seguridad web.

---

## Tabla de contenidos

* [Objetivo](#objetivo)
* [Aviso legal / Ética](#areas-de-estudio)
* [Tecnologías y herramientas](#tecnologías-y-herramientas)
* [Metodología utilizada](#metodología-utilizada)
* [Estructura del repositorio](#estructura-del-repositorio)
* [Contacto](#contacto)
* [Etiquetas](#etiquetas)

---

## Objetivo
Este repositorio funciona como mi portfolio de aprendizaje y práctica en ciberseguridad ofensiva.
Aquí documento:
- Laboratorios de seguridad web.
- Máquinas vulnerables de plataformas de entrenamiento.
- CTFs independientes
- Scripts desarrollados para automatización y enumeración.
- Notas técnicas sobre vulnerabilidades, metodologías y herramientas.
El objetivo es mantener un registro organizado de conocimientos, mejorar mis habilidades técnicas y demostrar experiencia práctica en pentesting.


---

## Áreas de estudio
### Seguridad Web
- SQL Injection
- Cross-Site Scripting (XSS)
- Access Control
- Authentication

### Pentesting
- Enumeración de servicios
- Explotación de vulnerabilidades
- Escalada de privilegios en Linux
- Post-Explotación

### Redes
- TCP/IP
- DNS
- HTTP/HTTPS
- SMB
  
---

## Tecnologías y herramientas
### Sistemas operativos
- Kali Linux
- Windows
- Ubuntu

### Herramientas
- Nmap
- BurpSuite
- ffuf
- Gobuster
- Metasploit
- Wireshark
- SQLMap

### Lenguajes
- Python
- Javascript
- Bash
  
---

## Metodología utilizada
La documentación sigue una metodología inspirada en PTES y procesos utilizados en auditorías de seguridad.
1. Reconocimiento
- Escaneos con Nmap
- Identificación de servicios, versiones y vectores iniciales
2. Enumeración
- Fuzzing con ffuf
- Análisis web con Burp Suite
- Enumeración SMB, FTP, SSH, etc.
- Recolección de credenciales y rutas vulnerables
3. Explotación
- Uso de exploits manuales o PoCs
- Metasploit cuando corresponde
- Inyección, RCE, LFI/RFI, fuerza bruta, etc.
4. Escalada de privilegios
- Análisis de permisos
- SUID, sudoers
- Servicios vulnerables
- Credenciales internas
5. Documentación
- Cada writeup incluye pasos claros, comandos utilizados y conclusiones técnicas.

---

## Estructura del repositorio

```
cybersecurity-labs/
│
├── TryHackMe/
│   ├── Easy/
│   │   ├── Vulnversity-THM.md
│   │   ├── Blue-THM.md
│   │   ├── BasicPentesting-THM.md
│   │   └── ColddBox-THM.md
│   └── (más niveles próximamente)
│
├── PortSwigger/
│   └── (walkthroughs futuros)
│
└── Plantillas y notas
```

---

## Contacto

**Mariano Marina**\
Estudiante de Licenciatura en Informática

---

## Etiquetas
#pentesting #tryhackme #ctf #writeups #cybersecurity  
#ethicalhacking #oscp #redteam #enumeration #privesc  
#infosec #walkthroughs #hackmyvm #offensivesecurity
