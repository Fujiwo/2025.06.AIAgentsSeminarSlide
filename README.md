# 2025.06.AIAgentsSeminarSlide

AIエージェントとMCP（Model Context Protocol）に関する開発者向けセミナー資料

## 概要

このリポジトリには、AIエージェントとMCP（Model Context Protocol）について説明するPowerPointプレゼンテーションが含まれています。Microsoft BUILD 2025での発表内容を基に、日本の開発者向けに作成されています。

## ファイル構成

- `AIエージェントとMCP_セミナー.pptx` - メインのプレゼンテーション資料
- `create_presentation.py` - プレゼンテーション作成用Pythonスクリプト

## 内容

プレゼンテーションは以下の内容を含みます：

### AIエージェント
- AIエージェントとは何か
- GitHub Copilot Agent Mode (Visual Studio Code)
- 類似ツール（Cline、Cursor）
- GitHub Copilot Coding Agent

### MCP（Model Context Protocol）
- MCPの概念と目的
- マルチエージェントオーケストレーション
- MCPサーバーの役割
- Claude Desktopでの利用
- .NETでのMCPサーバー開発
- Visual Studio Codeでの活用

### 背景
- Microsoft BUILD 2025の概要
- 「AIエージェントの時代」というテーマ
- 業界への影響と今後の展望

## 画像とソース

プレゼンテーションには以下のソースから引用した画像が含まれています：

- GitHub Copilot Coding Agent: https://www.publickey1.jp/2025/github-codingagent-01.png
- MCP概念図: https://www.publickey1.jp/2025/windows-support-mcp.png
- Satya Nadella at BUILD 2025: https://image.itmedia.co.jp/news/articles/2505/20/l_yu_satya.jpg

## 参考資料

- [Microsoft Build 2025 Keynote Summary - ITmedia NEWS](https://www.itmedia.co.jp/news/articles/2505/20/news097.html)
- [[速報] MicrosoftがWindowsでMCPサポートを発表 - Publickey](https://www.publickey1.jp/blog/25/windowsmcpaiwindows.html)

## 使用方法

プレゼンテーションを再生成する場合：

```bash
pip install python-pptx
python create_presentation.py
```