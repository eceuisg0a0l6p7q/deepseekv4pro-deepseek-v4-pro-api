# DeepSeek V4 Pro API (deepseek-v4-pro / deepseekv4pro) — llm guide with published pricing

> **input $1.0286; cached_input $0.2057; output $3.0857** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://go.apimart.ai/k-9be2f4)** · **[Get an API key](https://go.apimart.ai/k-b301b9)**

Everything here refers to **deepseek-v4-pro** — also written **deepseekv4pro** or **deepseek v4 pro**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `input` | $1.0286 |
| `cached_input` | $0.2057 |
| `output` | $3.0857 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $102.8571 |
| 1,000 | $1,028.5712 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/images/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"deepseek-v4-pro","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
