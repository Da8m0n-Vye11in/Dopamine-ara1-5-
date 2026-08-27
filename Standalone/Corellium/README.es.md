[Volver a la selección de idioma](../../README.md)

# Instalación de Dopamine en Corellium

1. Copie endpoint.sample.json a endpoint.json y agregue las credenciales de la cuenta Corellium; tenga en cuenta que se requiere ya sea la combinación usuario+contraseña o un token TOTP
2. Compile Dopamine
3. Ejecute `codesign -dvvvv on BaseBin/dopamine/dopamine`
4. Copie el CandidateCDHash y péguelo en Settings -> Trust Cache en la instancia de Corellium no jailbreakeada
5. Ejecute `env NODE_TLS_REJECT_UNAUTHORIZED=0 node dopamine.js install <Project> <Instance>` donde `Project` y `Instance` pueden ser un nombre o una ID
6. En la instancia, bajo "Port Forwarding", agregue un puerto: Device port = 22, Router port = 22, habilite expose port
7. Asegúrese de que el dispositivo esté conectado a la red Wi‑Fi
8. Bajo "Connect" puede encontrar la IP Wi‑Fi en la parte inferior
9. Ahora puede SSH al dispositivo usando `ssh mobile@<Wi-Fi IP>`

---
Nota de traducción: traducido por máquina y revisado por GitHub Copilot Chat Assistant
