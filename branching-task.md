# Задание «Ветвление, merge и rebase»

Схема веток: https://github.com/Alm798/Git/network

## Итог
- `branching/merge.sh` — цикл с `shift`, выводит каждый параметр отдельно.
- `branching/rebase.sh` — выводит `Next parameter: ...` для каждого параметра и `=====` в конце.

## Выполненные шаги
1. root-commit: `prepare for merge and rebase` в `main`.
2. Ветка `git-merge`: `merge: @ instead *`, затем `merge: use shift`.
3. Ветка `main`: правка `rebase.sh` (перешли на `"$@"` + `=====`).
4. Ветка `git-rebase`: создана от root-commit; коммиты `git-rebase 1`, `git-rebase 2`.
5. `git-rebase` → rebase на `main` с конфликтами, решено как в задании; force-push.
6. Fast-forward merge `git-rebase` → `main`. (И `git-merge` → `main` без конфликтов.)
