# Yellow RAT Lab - CyberDefenders

## Herramientas
- VirusTotal
- Red Canary (Threat Intel)

## ¿Qué pasó?
- Workstations infectadas con Yellow Cockatoo RAT (familia Solarmarker)
- Malware llegaba como DLL disfrazada con nombre GUID
- Filename: 111bc461-1ca8-43c6-97ed-911e0e69fdf8.dll
- Dejaba archivo de configuración: solarmarker.dat en AppData
- Compilado: 2020-09-24 18:26
- Primera vez visto en VirusTotal: 2020-10-15 02:47
- C2 server: https://gogohid.com

## Lo que aprendí
- Qué es threat intelligence
- Cómo investigar un hash en VirusTotal
- Por qué un malware tiene varios nombres (cada vendor lo nombra diferente)
- Qué es un RAT (Remote Access Trojan)
- Qué es un C2 server y por qué importa bloquearlo
- Cómo leer pestañas DETECTION, DETAILS, RELATIONS, BEHAVIOR en VirusTotal
- Uso de YARA rules para identificar familias de malware
- Importancia del compilation timestamp vs first submission
