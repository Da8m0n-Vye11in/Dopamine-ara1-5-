[Вернуться к выбору языка](../../README.md)

# Установка Dopamine на Corellium

1. Скопируйте endpoint.sample.json в endpoint.json и добавьте учетные данные для аккаунта Corellium, обратите внимание, что требуется либо комбинация имя+пароль, либо TOTP токен
2. Скомпилируйте Dopamine
3. Выполните `codesign -dvvvv on BaseBin/dopamine/dopamine`
4. Скопируйте CandidateCDHash и вставьте его в Settings -> Trust Cache на не взломанном экземпляре Corellium
5. Выполните `env NODE_TLS_REJECT_UNAUTHORIZED=0 node dopamine.js install <Project> <Instance>`, где `Project` и `Instance` могут быть именем или ID
6. В экземпляре в разделе "Port Forwarding" добавьте порт: Device port = 22, Router port = 22, включите expose port
7. Убедитесь, что устройство подключено к Wi‑Fi сети
8. В разделе "Connect" внизу можно найти Wi‑Fi IP
9. Теперь вы можете подключиться по SSH к устройству с помощью `ssh mobile@<Wi-Fi IP>`

---
Примечание перевода: машинный перевод + вычитка GitHub Copilot Chat Assistant
