# Amadey APT-C-36 Lab - CyberDefenders

## Herramientas
- Volatility 3 (análisis forense de memoria)

## ¿Qué pasó?
- EDR alertó actividad sospechosa fuera de horas en workstation Windows
- Infección con Amadey Trojan Stealer
- Proceso malicioso: lssass.exe (imita lsass.exe legítimo - técnica Masquerading T1036)
- Ubicación: C:\Users\0xSh3rl0ck\AppData\Local\Temp\925e7e99c5\lssass.exe
- C2 server: 41.75.84.12 (puerto 80, HTTP)
- Descargó 2 payloads adicionales: clip64.dll y cred64.dll
- DLL principal: C:\Users\0xSh3rl0ck\AppData\Roaming\116711e5a2ab05\clip64.dll
- Ejecutó las DLLs vía rundll32.exe (Living Off the Land - T1218.011)
- Persistencia: Scheduled Task en C:\Windows\System32\Tasks\lssass.exe

## Lo que aprendí
- Qué es memory forensics y por qué se usa
- Volatility 3: pslist, pstree, cmdline, netscan, filescan
- Técnica Masquerading (nombres parecidos a procesos legítimos)
- Living Off the Land Binaries (LOLBins) - abusar de binarios legítimos
- Persistencia vía Scheduled Tasks
- Cómo se lee netscan (origen → destino, PID, proceso)
- AppData\Roaming como ubicación típica de payloads
