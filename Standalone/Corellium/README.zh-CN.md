[返回語言選擇](../../README.md)

# 在 Corellium 上安装 Dopamine

1. 复制 endpoint.sample.json 为 endpoint.json，并添加 Corellium 帐户的凭据，注意需要用户名+密码组合或 totp 令牌之一
2. 编译 Dopamine
3. 运行 `codesign -dvvvv on BaseBin/dopamine/dopamine`
4. 复制 CandidateCDHash 并将其粘贴到非越狱 Corellium 实例的 Settings -> Trust Cache 中
5. 运行 `env NODE_TLS_REJECT_UNAUTHORIZED=0 node dopamine.js install <Project> <Instance>`，其中 `Project` 和 `Instance` 可以是名称或 ID
6. 在实例的 "Port Forwarding" 下添加端口：Device port = 22，Router port = 22，启用 expose port
7. 确保设备已连接到 Wi‑Fi 网络
8. 在 "Connect" 下可以在底部找到 Wi‑Fi IP
9. 现在可以使用 `ssh mobile@<Wi-Fi IP>` SSH 登录设备

---
翻译说明：机器翻译 + GitHub Copilot Chat Assistant 校对
