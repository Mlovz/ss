# Contributing

## TL;DR

1. Создайте ветку от `main`: `feat/<scope>-<topic>`
2. Маленькие PR (<400 строк), один смысл — один PR
3. Коммиты по Conventional Commits: `feat(auth): ...`
4. Локально: `pnpm typecheck && pnpm lint && pnpm test && pnpm build`
5. Обновите доку/сторибуки, добавьте скриншоты в PR

## Среда

-   Node LTS, pnpm, Nx
-   `pnpm i` после клонирования, затем `pnpm start` для `apps/web`

## Архитектура

-   Слои: `ui` → `feature-*` → `data-access` → `util`
-   Запрещены обратные зависимости (см. ESLint `@nx/enforce-module-boundaries`)

## Тестирование

-   Unit ≥ 80% по критичным lib, e2e-smoke обязателен для UI‑флоу

## Коммиты

-   `feat|fix|chore|refactor|docs|test|build|ci(scope): message`

## PR

-   Ветка актуальна с `main`
-   Все чек‑листы из шаблона PR — выполнены
-   CODEOWNERS добавлены в ревьюеры
