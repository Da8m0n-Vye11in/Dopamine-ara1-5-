[返回語言選擇](../../README.md)

# 在 Corellium 上安裝 Dopamine

1. 將 endpoint.sample.json 複製為 endpoint.json，並新增 Corellium 帳戶的憑證，注意需要使用者名+密碼組合或 totp 令牌其一
2. 編譯 Dopamine
3. 執行 `codesign -dvvvv on BaseBin/dopamine/dopamine`
4. 複製 CandidateCDHash 並將其貼入非越獄 Corellium 實例的 Settings -> Trust Cache
5. 執行 `env NODE_TLS_REJECT_UNAUTHORIZED=0 node dopamine.js install <Project> <Instance>`，其中 `Project` 和 `Instance` 可以是名稱或 ID
6. 在實例的 "Port Forwarding" 下新增端口：Device port = 22，Router port = 22，啟用 expose port
7. 確保裝置已連接到 Wi‑Fi 網路
8. 在 "Connect" 下方能在底部找到 Wi‑Fi IP
9. 現在可以使用 `ssh mobile@<Wi-Fi IP>` SSH 登入裝置

---
翻譯說明：機器翻譯 + GitHub Copilot Chat Assistant 校對
