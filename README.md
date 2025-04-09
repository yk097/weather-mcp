# weather-mcp

MCPクライアントに天気情報のコンテキストを追加するMCPサーバです。

## 環境構築
```bash
$ git clone https://github.com/yk097/weather-mcp.git
$ cd weather-mcp
$ npm install
$ npm run build
```

## MCPクライアントへの設定
```json
{
  "mcpServers": {
    "weather": {
      "command": "node",
      "args": [
        "/PATH/TO/weather-mcp/build/index.js"
      ]
    }
  }
}
```
nodeをnodebrewで入れている場合は、以下のように絶対パスで指定してください。
```json
"command": "/PATH/TO/.nodebrew/current/bin/node",
```

