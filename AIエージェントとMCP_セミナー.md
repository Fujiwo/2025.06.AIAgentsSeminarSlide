# AIエージェントとMCP (Model Context Protocol)

## 開発者向けセミナー
### 2025年6月

---

## AIエージェントとは？

AIエージェントは、ユーザーの代わりに行動し、タスクを実行するAIシステムです

### 主要な例：
- GitHub Copilot Agent Mode (Visual Studio Code)
  - 類似ツール: Cline、Cursor
- GitHub Copilot Coding Agent

---

## AIエージェントエコシステム

```
AIエージェントエコシステム:

                [Human User]
                     ↓
               [AI Assistant]
                ↙    ↓    ↘
        [Code Agent] [Data Agent] [UI Agent]
             ↓           ↓           ↓
          [GitHub]   [Database]   [Browser]
             ↓           ↓           ↓
        [Repository] [Analytics] [Web Apps]

全てのエージェントがMCPプロトコルで相互接続
```

---

## GitHub Copilot Coding Agent

![GitHub Copilot Coding Agent](https://www.publickey1.jp/2025/github-codingagent-01.png)

*出典: GitHub Copilot Coding Agent発表資料*

---

## MCP (Model Context Protocol) とは？

AIエージェント同士が連携するためのプロトコル

- Microsoftが全面採用を発表
  - Windows、Microsoft 365などの主要製品でサポート
  - AIエージェント間のスムーズな情報交換と連携を実現

---

## MCP概念図

![MCP概念図](https://www.publickey1.jp/2025/windows-support-mcp.png)

*出典: [速報] MicrosoftがWindowsでMCPサポートを発表、AIエージェントがWindowsやアプリと連携可能に - Publickey*  
*https://www.publickey1.jp/blog/25/windowsmcpaiwindows.html*

---

## Microsoft BUILD 2025

- 2025年5月20-23日開催
- テーマ: 「AIエージェントの時代」
  - CEO Nadellaが従来のAIモデルからAIエージェントへの進化を強調

![Satya Nadella at BUILD 2025](https://image.itmedia.co.jp/news/articles/2505/20/l_yu_satya.jpg)

---

## 主な発表内容

- MCPサーバーレジストリの提供
- WindowsでのMCPサポート
- Microsoft 365でのMCPサポート
- GitHub Copilot Coding Agentの発表

---

## マルチエージェントオーケストレーション

複数のAIエージェントが連携して複雑なタスクを実行

- 各エージェントが専門的な役割を担当
- MCPプロトコルにより効率的な情報共有
- サービス、OS、アプリケーション、Webページとの連携

### マルチエージェント構成例:

```
[UI Agent] ←→ [MCP Protocol] ←→ [API Agent]
     ↕                              ↕
[User Interface]              [External Services]
     ↕                              ↕  
[Analytics Agent] ←→ [MCP] ←→ [Database Agent]
```

---

## MCPサーバー

AIエージェントと外部システム間の橋渡し役

- 様々なサービスやAPIとの接続を提供
- 標準化されたインターフェースで一貫性を保証
- Claude Desktopでの利用デモも提供

### MCPサーバーアーキテクチャ:

```
[AI Agent] ←→ [MCP Protocol] ←→ [MCP Server]
                                      ↓
                               [Adapter Layer]
                                      ↓
                    [Database] [API] [File System] [Web Services]
```

---

## MCPサーバー実装例

![MCP Implementation Example](https://docs.anthropic.com/en/docs/_next/image?url=%2Fen%2Fdocs%2F_next%2Fstatic%2Fmedia%2Fmcp-architecture.bfaa5e8c.png&w=1080&q=75)

*出典: Anthropic MCP Documentation - Claude Desktop MCP Integration Example*

---

## .NETでのMCPサーバー開発

Microsoft環境での開発支援

- .NET Framework/Coreでの実装
- 豊富なライブラリとツールチェーンの活用
- 実践的なデモンストレーション付き

---

## Visual Studio Codeでの利用

開発者にとって身近な環境での実装

- 拡張機能によるMCPサポート
- AIエージェントとの直接的な連携
- 実際のワークフローでのデモンストレーション

---

## 未来への展望

アプリケーションとサービスの性質が大きく変化

- 近年提案されているマイクロアーキテクチャと同様の進化
  - HTTP/HTTPSでマイクロサービスを接続するように
  - MCPでAIエージェントを接続
- Microsoft、その他多くのIT企業がMCPを採用

---

## まとめ

- AIエージェントの時代が到来
  - MCPがAIエージェント連携の標準プロトコルに
  - 開発者は新しいアーキテクチャパターンへの対応が必要
  - 実践的なデモと開発環境の整備が進行中

---

## 参考資料

### Microsoft Build 2025 公式情報
- https://www.itmedia.co.jp/news/articles/2505/20/news097.html
- https://www.publickey1.jp/blog/25/windowsmcpaiwindows.html

### GitHub Copilot 関連
- https://github.com/features/copilot
- https://docs.github.com/en/copilot

### MCP (Model Context Protocol) 関連
- https://modelcontextprotocol.org/
- https://github.com/modelcontextprotocol

### AI エージェント関連
- https://openai.com/research/agents
- https://claude.ai/
- https://cursor.sh/
- https://github.com/cline/cline

---

## 画像とソース

プレゼンテーションには以下のソースから引用した画像が含まれています：

- **GitHub Copilot Coding Agent**: https://www.publickey1.jp/2025/github-codingagent-01.png
- **MCP概念図**: https://www.publickey1.jp/2025/windows-support-mcp.png
- **Satya Nadella at BUILD 2025**: https://image.itmedia.co.jp/news/articles/2505/20/l_yu_satya.jpg
- **MCP Implementation Example**: https://docs.anthropic.com/en/docs/_next/image?url=%2Fen%2Fdocs%2F_next%2Fstatic%2Fmedia%2Fmcp-architecture.bfaa5e8c.png&w=1080&q=75

## 使用方法

プレゼンテーションを再生成する場合：

```bash
pip install python-pptx requests
python create_presentation.py
```

このMarkdownファイルは、同じ内容をドキュメント形式で提供します。