[언어 선택으로 돌아가기](../../README.md)

# MachOMerger

두 개의 MachO 바이너리를 하나로 병합합니다. 현재 지원되는 유일한 사용 사례는 dylib를 dyld에 병합하는 것입니다.

# 요구사항

- 주입할 dylib는 `-Xlinker -add_split_seg_info -Xlinker -no_auth_data`로 컴파일되어야 합니다.

---
번역: 기계 번역 + GitHub Copilot Chat Assistant 교정
