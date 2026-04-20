# BrandEdge Premium — Posit Connect Deploy

Shiny app bundle for **BrandEdge 旗艦版（品牌印記引擎）**.

## Deploy

Posit Connect Cloud (https://connect.posit.cloud/) reads this repo and starts Shiny
via the top-level `app.R` (which is a copy of `app_brandedge.R`).

### Required environment variables (Connect → Content → Variables)

| Name | Purpose |
|------|---------|
| `PGHOST` | Postgres host (Supabase direct or pooler) |
| `PGPORT` | `5432` (session pooler or direct) |
| `PGUSER` | `postgres` (direct) or `postgres.<project_ref>` (pooler) |
| `PGPASSWORD` | Postgres password (Secret) |
| `PGDATABASE` | `postgres` |
| `PGSSLMODE` | `require` |
| `OPENAI_API_KEY` | OpenAI key (Secret) |

User accounts are stored in the `public.users` table (Supabase).

## Local dev

```r
# Fill in .env using .env.example as template, then:
Rscript app.R
```
