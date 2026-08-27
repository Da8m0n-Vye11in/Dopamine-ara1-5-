[返回語言選擇](../../README.md)

# MachOMerger

將兩個 MachO 二進位檔合併為一個。目前唯一受支援的用例是將 dylib 合併到 dyld 中。

# 要求

- 要注入的 dylib 必須使用 `-Xlinker -add_split_seg_info -Xlinker -no_auth_data` 編譯

---
翻譯說明：機器翻譯 + GitHub Copilot Chat Assistant 校對
