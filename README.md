# Route Rules

Clash 分流规则文件，数据源来自 [Loyalsoldier/clash-rules](https://github.com/Loyalsoldier/clash-rules)。

## 使用

在 Clash Nyanpasu / Clash.Meta 配置中引用：

```yaml
rule-providers:
  gfw-rules:
    type: http
    url: "https://raw.githubusercontent.com/sheepix/route-rules/master/clash-rules.yaml"
    interval: 86400
    path: ./providers/gfw-rules.yaml
    format: yaml
```

## 更新

- 数据源: [Loyalsoldier/clash-rules](https://github.com/Loyalsoldier/clash-rules)
- 更新频率: 每天凌晨 3 点 (Cron)
- 自动推送: 更新后自动提交到本仓库

## 规则文件

| 文件 | 内容 |
|------|------|
| `clash-rules.yaml` | 完整的 Clash 分流规则 (12 万+ 条) |

## 规则来源

| 来源 | 内容 |
|------|------|
| lancidr.txt | 局域网 IP 直连 |
| direct.txt | 国内网站直连 |
| gfw.txt | GFW 代理规则 |
| telegramcidr.txt | Telegram IP 段 |
