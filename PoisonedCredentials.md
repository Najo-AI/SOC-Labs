# PoisonedCredentials Lab - CyberDefenders

## Herramientas
- Wireshark

## ¿Qué pasó?
- Ataque LLMNR/NBT-NS Poisoning en red Windows
- Máquina víctima (192.168.232.162) buscó FILESHAARE (typo de FILESHARE)
- Atacante (192.168.232.215) respondió haciéndose pasar por ese recurso
- Segunda víctima (192.168.232.176) también cayó en el envenenamiento
- Atacante capturó credenciales NTLM del usuario comprometido
- Acceso posterior vía SMB

## Lo que aprendí
- Qué es LLMNR/NBT-NS Poisoning y cómo funciona
- Filtros de Wireshark: ip.addr, llmnr, nbns, ntlmssp
- Qué es SMB (compartir archivos en redes Windows)
- Qué es NTLMSSP (autenticación Windows en red)
- Cómo identificar la máquina rogue en un pcap
- Cómo se capturan credenciales en este tipo de ataques
