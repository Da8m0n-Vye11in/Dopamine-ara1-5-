[Вернуться к выбору языка](../../README.md)

# MachOMerger

Слияние двух MachO бинарников в один. В данный момент единственный поддерживаемый сценарий — внедрение dylib в dyld.

# Требования

- Внедряемый dylib *должен* быть скомпилирован с `-Xlinker -add_split_seg_info -Xlinker -no_auth_data`

---
Примечание перевода: машинный перевод + вычитка GitHub Copilot Chat Assistant
