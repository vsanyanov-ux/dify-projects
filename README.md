# dify-projects
Dify AI workflows and applications - DSL exports and documentation

## Структура репозитория

```
dify-projects/
├── dsl/              # DSL-файлы экспортированных приложений
│   └── stp-workflow.dsl.yaml
├── docs/             # Документация и описания
│   └── stp-workflow.md
└── README.md         # Этот файл
```

## Проекты

### СТП (Система управления проектами)
Chatflow для управления проектами с интеграцией knowledge base.

**DSL:** `dsl/stp-workflow.dsl.yaml`

## Как использовать

### Импорт приложения в Dify

1. Перейдите в Studio → Apps
2. Нажмите "Import DSL"
3. Загрузите файл из папки `dsl/`
4. Настройте переменные окружения и API-ключи:
   - Модель LLM (Gemini, OpenAI и т.п.)
   - Knowledge base connections
   - Прочие интеграции

### Обновление DSL

1. В Dify откройте приложение
2. Нажмите "Export DSL"
3. Сохраните файл в папку `dsl/`
4. Закоммитьте изменения:
```bash
git add dsl/
git commit -m "Update: описание изменений"
git push
```

## Важно

- DSL-файлы **НЕ содержат** API-ключи и секреты
- После импорта нужно вручную добавить credentials в Workspace Settings
- Содержимое knowledge base не экспортируется, только ссылки
