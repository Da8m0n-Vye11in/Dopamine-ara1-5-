[Volver a la selección de idioma](../../README.md)

# MachOMerger

Fusiona dos binarios MachO en uno. El único caso de uso compatible en este momento es fusionar un dylib en dyld.

# Requisitos

- El dylib a inyectar *debe* compilarse con `-Xlinker -add_split_seg_info -Xlinker -no_auth_data`

---
Nota de traducción: traducido por máquina y revisado por GitHub Copilot Chat Assistant
