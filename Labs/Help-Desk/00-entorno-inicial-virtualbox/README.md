# LAB 00 - Entorno inicial en VirtualBox

## Objetivo
Diseñar y desplegar un entorno IT corporativo simulado usando VirtualBox, que sirva como base para labs de helpdesk, administración de sistemas y seguridad.

El entorno incluye:

- Red interna corporativa con acceso a Internet
- Servidor Linux con sistema de tickets (osTicket)
- Estaciones Windows (usuario y administrador)
- Buenas prácticas de administración y documentación


## Tecnologías utilizadas
- VirtualBox
- Ubuntu Server
- Windows 10 Home
- Windows 10 Pro
- osTicket
- Redes NAT + Red Interna


## Estructura de la carpeta del lab

00-entorno-inicial-virtualbox/
├── README.md
├── diagrama-red.png
├── configuracion-red.md
├── maquinas/
│   ├── ubuntu-osticket.md
│   ├── windows-usuario.md
│   └── windows-admin.md
└── verificaciones.md


## Diseño de red

Se simula una pequeña empresa con LAN interna y salida a Internet.

### Adaptadores de red en VirtualBox

- Adaptador 1: NAT (acceso a Internet)
- Adaptador 2: Red interna

### Esquema lógico de la red
