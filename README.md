# mcp-client-python

これは、[(Model Context Protocol（MCP)](https://modelcontextprotocol.io/quickstart/client) を使って、Claude
APIと天気情報サーバーを接続するPythonクライアントです。

自然言語による質問に対し、必要に応じてツール（`get_forecasts` や `get_result`）を呼び出します。

参考： [公式Quickstart](https://modelcontextprotocol.io/quickstart/client)

使用するサーバー： [weather-server-python](https://github.com/maa0917/weather-server-python)

## 機能

- Cloude 3.5 Sonnet と連携して自然言語応答
- MCPプロトコル経由でツールを呼び出し
- 米国の天気予報を取得

## セットアップ

1. リポジトリをクローン

```bash
git clone https://github.com/maa0917/mcp-client-python.git
cd mcp-client-python
```

2. 仮想環境を作成してアクティブ化

```bash
python -m venv .venv
source .venv/bin/activate
```

3. .env ファイルを作成し、AnthropicのAPIキーを設定

```bash
ANTHROPIC_API_KEY=<your key here>
```

## 実行方法

```bash
uv run client.py path/to/server.py
```

## 使い方例

```bash
Query: What are the weather alerts in California?
```

## 終了方法

- quit と入力する
- もしくは Ctrl + C で終了
