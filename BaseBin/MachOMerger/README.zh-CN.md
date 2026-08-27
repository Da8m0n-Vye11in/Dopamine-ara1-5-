[返回語言選擇](../../README.md)

# MachOMerger

将两个 MachO 二进制合并为一个。目前唯一受支持的用例是将 dylib 合并到 dyld 中。

# 要求

- 要注入的 dylib 必须使用 `-Xlinker -add_split_seg_info -Xlinker -no_auth_data` 编译

---
翻译说明：机器翻译 + GitHub Copilot Chat Assistant 校对
