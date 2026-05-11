# Oski Lab - CyberDefenders

## Herramientas
- VirusTotal
- Any.Run (sandbox)
- MITRE ATT&CK

## ¿Qué pasó?
- Atacante envió email con PPT malicioso
- Al abrirlo descargó malware Stealc
- El malware se conectó a C2: http://171.22.28.221/5c06c05b7b34e8e6.php
- Robó contraseñas del navegador usando sqlite3.dll
- Borró sus DLLs de C:\ProgramData para no dejar rastro
- Se autoeliminó a los 5 segundos

## Lo que aprendí
- Qué es un hash y para qué sirve
- Qué es un sandbox (Any.Run)
- Qué es un servidor C2
- Por qué el malware busca sqlite3.dll (robo de credenciales)
- Qué es RC4 y cifrado de configuración
- Cómo usar MITRE ATT&CK para identificar técnicas (T1555)
- Cómo el malware se autoeliminan para evadir detección
