# SpeechRecognitionTool GPU Runtime

此仓库仅分发 SpeechRecognitionTool 的 Windows x64 GPU Runtime 包，不存放应用源码或模型权重。

支持 Qwen3-ASR、GLM-ASR-Nano 和 MOSS-Transcribe-Diarize。使用支持自动修复的应用版本，在「设置 → 常规」选择对应 Runtime，点击「一键修复 Runtime」，应用将自动下载匹配版本、校验、安装和自检。

每个 Release 的标签为 `v<应用版本>`。包清单为 `SpeechRecognitionTool-<版本>-gpu-asr-<qwen|glm|moss>-win-x64.package.json`，分卷为同名前缀的 `.zip.part001` 等文件。请保留全部分卷；应用会校验各分卷、重组归档以及展开后的文件树。

Runtime 包含嵌入式 Python、固定依赖及 GPU Worker，不包含 NVIDIA 驱动或识别模型。各第三方组件保留包内许可证；安装成功不代表特定显卡与模型已通过识别验收。