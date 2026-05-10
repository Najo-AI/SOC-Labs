# WebStrike Lab - CyberDefenders

## Herramientas
- Wireshark

## ¿Qué pasó?
- Atacante desde IP 117.11.88.124 atacó servidor web
- Subió web shell (image.jpg.php) usando file upload bypass
- Estableció reverse shell por puerto 8080
- Intentó exfiltrar /etc/passwd

## Lo que aprendí
- Filtrar HTTP en Wireshark
- Diferencia entre GET y POST
- Qué es un web shell
- Qué es una reverse shell
- Cómo seguir HTTP Stream y TCP Stream
