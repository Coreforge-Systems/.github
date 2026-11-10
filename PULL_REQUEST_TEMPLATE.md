[Русский](https://github.com/Coreforge-Systems/.github/blob/main/PULL_REQUEST_TEMPLATE_RU.md) | [English](https://github.com/Coreforge-Systems/.github/blob/main/PULL_REQUEST_TEMPLATE_EN.md)

## Краткое описание / Summary

Опишите, что изменяет этот pull request и зачем. / Describe what this pull request changes and why.

## Тип изменения / Type of change

- [ ] Новая возможность / Feature
- [ ] Исправление ошибки / Bug fix
- [ ] Рефакторинг / Refactoring
- [ ] Тесты / Tests
- [ ] Документация / Documentation
- [ ] Сборка / CI / Build
- [ ] Несовместимое изменение API или протокола / Breaking API or protocol change

## Затронутые области / Affected areas

- [ ] Ядро / предметная область / Core / domain
- [ ] Протокол / Protocol
- [ ] Транспорт / Transport
- [ ] Симулятор / Simulator
- [ ] Интерфейс настольного приложения / Desktop UI
- [ ] Прошивка / Firmware
- [ ] Хранение данных / отчёты / Storage / reporting
- [ ] Документация / Documentation

## Проверка / Validation

Опишите, как тестировалось изменение. / Describe how the change was tested.

## Влияние на устройство / протокол / Device / protocol impact

Влияет ли это изменение на формат обмена по протоколу, публичный API C++, схемы, совместимость устройств или поведение, от которого зависит безопасность? Если да, опишите путь миграции.

Does this change affect the wire protocol, public C++ API, schemas, device compatibility, or safety-sensitive behavior? If yes, describe the migration path.

## Контрольный список / Checklist

- [ ] Сборка завершается успешно / Build succeeds
- [ ] Соответствующие тесты проходят / Relevant tests pass
- [ ] Нет новых предупреждений компилятора / No new compiler warnings
- [ ] Рассмотрены ошибочные сценарии / Error paths were considered
- [ ] Секреты и конфиденциальные данные клиентов не включены / No secrets or sensitive customer data are included
- [ ] Документация обновлена там, где это требуется / Documentation was updated when required
- [ ] Несовместимые изменения явно задокументированы / Breaking changes are explicitly documented
