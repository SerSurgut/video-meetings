# video-meetings

Монорепозиторий (pnpm workspaces):

| Приложение | Стек    | Порт | Путь       |
| ---------- | ------- | ---- | ---------- |
| `web`      | Next.js | 3000 | `apps/web` |
| `api`      | NestJS  | 4000 | `apps/api` |

## Требования

- Node.js >= 24 (см. `.nvmrc`)
- pnpm >= 11

## Команды (из корня)

```bash
pnpm install        # установка зависимостей
pnpm dev            # web + api параллельно
pnpm dev:web        # только web
pnpm dev:api        # только api
pnpm build          # сборка всех приложений
pnpm lint           # ESLint во всех приложениях
pnpm lint:fix       # ESLint --fix
pnpm typecheck      # tsc --noEmit
pnpm test           # тесты (api)
pnpm format         # Prettier --write
pnpm format:check   # Prettier --check
```

Команды отдельного приложения: `pnpm --filter web <script>` / `pnpm --filter api <script>`.
