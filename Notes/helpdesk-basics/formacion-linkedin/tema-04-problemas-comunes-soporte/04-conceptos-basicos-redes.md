# Conceptos básicos de redes

En entornos de HelpDesk es habitual recibr incidencias relacionadas con problemas de red. Estas incidencias suelen dividirse en dos grandes categorías, cada una con un enfoque de resolución distinto.


## Tipos de problemas de red

### 1. Problemas de red corporativa
Son incidencias que afectan a la red de la empresa y, normalmente, a múltiples usuarios.

Características:
- Pueden afectar a un departamento o a toda la organización
- Suelen requerir escalado si el impacto es elevado
- El técnico de HelpDesk actúa como primer filtro antes de escalar al equipo de redes.


### 2. Problemas de red doméstica
Son incidencias de usuarios que trabajan desde casa.

Características:
- Son más difíciles de resolver porque el técniico no está físicamente presente
- Suelen estar relacionados con problemas de Wi-Fi
- No siempre es posible conectarse remotamente
- El técnico debe guiar al usuario paso a paso durante la resolución
- Si no se resuelve, será necesario enviar a un técnico


## Esquema de decisiones ante un problema de red

1. Entra una llamada o ticket por un problema de red.
2. Se utilizan herramientas de IP para intentar diagnosticar el problema.
3. ¿El problema se resuelve?
   - **Sí** -> Se cierra el ticket.
   - **No** -> Se escala al equipo correspondiente.
     - Equipo de red corporativa si el usuario está en la red de la empresa.
     - Equipo de soporte doméstico si el usuario trabaja desde casa.
4. El equipo correspondiente determina si el problema es:
   - Cableado
   - Inalámbrico
   y actúa en consecuencia.


## Herramientas básicas de red

### ipconfig
Muestra información básica de la configuración de red del sistema.

Permite comprobar, entre otras cosas:
- Si el usuario tiene dirección IP asignada
- Si la configuración de red es válida


### ping
Envía solicitudes de eco ICMP a un dispositivo remoto.

Usos comunes:
- Verificar si un dispositivo está activo
- Comprobar conectividad con otros equipos
- Hacer ping a un dominio para verificar el funcionamiento del DNS


### ipconfig /all
Muestra información detallada de la configuración de red.

Usos comunes:
- Identificar el servidor DNS configurado
- Verificar si el servidor DNS responde correctamente
- Detectar problemas de DNS en redes corporativas o domésticas

En el caso de usuarios domésticos, los problemas de DNS suelen estar relacionados con el router del proveedor de internet (ISP).


### tracert
Muestra la ruta que sigue los paquetes hasta un destino específico.

Usos comunes:
- Identificar en qué punto de la red se interrumpe la conexión
- Localizar problemas de enrrutamiento
- Analizar la conectividad hacia paginas web o servidores externos
