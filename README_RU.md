[Русский](README_RU.md) | [English](README_EN.md)

# Coreforge Systems · .github

Общие для организации настройки GitHub и документы сообщества **Coreforge Systems**.

## Назначение

Общие настройки по умолчанию для репозиториев Coreforge Systems:

- публичный профиль организации;
- правила участия в разработке;
- правила оформления pull request;
- формы issues;
- порядок сообщения об уязвимостях;
- рекомендации по получению поддержки.

Отдельные репозитории проектов могут переопределять эти настройки, если требуются более строгие правила.

## Структура

```text
.github/
├── README.md
├── README_RU.md
├── README_EN.md
├── profile/
│   ├── README.md
│   ├── README_RU.md
│   └── README_EN.md
├── ISSUE_TEMPLATE/
│   ├── bug_report.yml
│   ├── feature_request.yml
│   ├── architecture_proposal.yml
│   └── config.yml
├── CONTRIBUTING.md
├── CONTRIBUTING_RU.md
├── CONTRIBUTING_EN.md
├── SECURITY.md
├── SECURITY_RU.md
├── SECURITY_EN.md
├── SUPPORT.md
├── SUPPORT_RU.md
├── SUPPORT_EN.md
├── PULL_REQUEST_TEMPLATE.md
├── PULL_REQUEST_TEMPLATE_RU.md
└── PULL_REQUEST_TEMPLATE_EN.md
```

Файлы без языкового суффикса сохраняют стандартные точки входа GitHub. Полные документы доступны на [русском](README_RU.md) и [английском](README_EN.md); стандартный шаблон pull request остаётся двуязычным и содержит все поля.

Основной продукт, который сейчас находится в разработке, — **DevicePilot**.
