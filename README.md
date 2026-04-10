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

- 数据源: [Loyalsoldier/clash-rules](https://github.com/Loyalsoldier/clash-rules) (每日更新)
- 本仓库: 服务器每天凌晨 3 点自动更新并推送

## 规则文件

| 文件 | 内容 |
|------|------|
| `clash-rules.yaml` | 完整的 Clash 分流规则 (12 万+ 条) |
